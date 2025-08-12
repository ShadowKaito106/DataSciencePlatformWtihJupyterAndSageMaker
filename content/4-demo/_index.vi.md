---
title : "Demo chạy thử"
date: "2025-08-12"
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

#### Demo chạy thử
1. Truy cập vào **JupyterLab** tại SageMaker Unified Studio  
    + Nhấn **Python 3(ipykernel) notebook**.

![DM](datascienceplatformwtihjupyterandsagemaker/images/4.demo/001-Demo.png)

2. Tại trang notebook của bạn  
   + Sao chép đoạn code sau và dán vào một ô trống

```
from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier
import joblib
import tarfile

# 1. Train model
iris = load_iris()
X_train, X_test, y_train, y_test = train_test_split(iris.data, iris.target, random_state=42)
clf = RandomForestClassifier()
clf.fit(X_train, y_train)

# 2. Lưu model
joblib.dump(clf, "model.joblib")

# 3. Đóng gói thành tar.gz (đúng chuẩn SageMaker)
with tarfile.open("iris-model.tar.gz", "w:gz") as tar:
    tar.add("model.joblib")
```

   
   + Nhấn nút **Run**.  
   + Nếu xuất hiện 2 file **iris-model.tar.gz** và **model.joblib** nghĩa là đã chạy thành công.

![DM](datascienceplatformwtihjupyterandsagemaker/images/4.demo/002-Demo.png)

3. Ở một ô trống khác  
   + Sao chép đoạn code sau và dán vào đó


```
import tarfile
import joblib
import numpy as np

# Decompress the model file
with tarfile.open("iris-model.tar.gz", "r:gz") as tar:
    tar.extractall(".")

# Load the trained model
model = joblib.load("model.joblib")


random_matrix = np.random.rand(4, 4) * 5

print("Generated 4x4 matrix:")
print(random_matrix)

# Attempt to use the matrix for prediction
try:
    predictions = model.predict(random_matrix)
    print("\nPredictions:", predictions)
except ValueError as e:
    print("\nAn error occurred:", e)
    print("\nReason: Your model was trained on data with a different number of features (likely 4).")
    print("The model's input shape must match the number of features it was trained on.")
    print("A 10x10 matrix is not a valid input shape for a model expecting 4 features per sample.")
```
    + Nhấn nút **Run**.

![DM](datascienceplatformwtihjupyterandsagemaker/images/4.demo/003-Demo.png)

4. Nếu xuất hiện kết quả tương tự như ma trận và dự đoán dưới đây, nghĩa là chạy thành công.

![DM](datascienceplatformwtihjupyterandsagemaker/images/4.demo/004-Demo.png)