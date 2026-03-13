# Fashion-MNIST Clothing Classification

## Giới thiệu

Dự án này xây dựng mô hình học sâu để **nhận dạng quần áo và giày dép thời trang** từ bộ dữ liệu Fashion-MNIST.
Mô hình được huấn luyện bằng thư viện PyTorch và chạy trên GPU của Google Colab.

## Dataset

Fashion-MNIST là bộ dữ liệu hình ảnh gồm **70.000 ảnh grayscale** kích thước **28x28 pixel**, được chia thành:

* **60.000 ảnh huấn luyện**
* **10.000 ảnh kiểm tra**


## Công nghệ sử dụng

* Python
* PyTorch
* NumPy
* Matplotlib
* Google Colab GPU

## Kiến trúc mô hình

Mô hình sử dụng **Neural Network (Fully Connected Network)**.

Cấu trúc:

Input Layer
→ Flatten (28x28 → 784)
→ Linear Layer
→ ReLU Activation
→ Linear Layer
→ Output Layer (10 classes)

## Huấn luyện mô hình

Các tham số huấn luyện:

* Loss Function: CrossEntropyLoss
* Optimizer: SGD / Adam
* Epochs: 20
* Batch Size: 32

Quá trình huấn luyện cho thấy **Loss giảm dần** và **Accuracy tăng dần theo số epoch**.

## Kết quả

Sau khi huấn luyện mô hình:

* Training Accuracy ≈ **88% – 90%**

Mô hình có khả năng phân loại chính xác các loại quần áo và giày dép trong bộ dữ liệu Fashion-MNIST.

## Biểu đồ kết quả

Trong quá trình huấn luyện, các biểu đồ sau được hiển thị:

* **Loss over Epochs**
* **Accuracy over Epochs**

Các biểu đồ này giúp quan sát quá trình học của mô hình.

## Cách chạy chương trình

1. Mở notebook trên Google Colab
2. Bật GPU

Runtime → Change runtime type → GPU

3. Chạy các bước:

* Load dataset Fashion-MNIST
* Tiền xử lý dữ liệu
* Huấn luyện mô hình
* Hiển thị biểu đồ Loss và Accuracy
* Kiểm tra dự đoán của mô hình

## Kết luận

Mô hình neural network đơn giản có thể đạt độ chính xác gần **90%** trên bộ dữ liệu Fashion-MNIST.
Điều này cho thấy học sâu có khả năng trích xuất đặc trưng hiệu quả từ dữ liệu hình ảnh.

## Tác giả

Student Project – Deep Learning Lab
