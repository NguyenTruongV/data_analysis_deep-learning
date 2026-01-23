
---

## 🧠 Mô tả dữ liệu
Dataset bao gồm thông tin của nhiều cá nhân với các thuộc tính:
- `Id`: Mã bệnh nhân  
- `Firstname`, `Lastname`: Tên  
- `Age`: Tuổi  
- `Weight`: Cân nặng  
- `Pulserate`: Nhịp tim theo các khoảng thời gian và giới tính  

Dữ liệu ban đầu tồn tại nhiều vấn đề như:
- Thiếu header
- Giá trị thiếu
- Đơn vị không nhất quán (lbs / kgs)
- Dữ liệu dạng wide cần chuyển sang long format
- Ký tự không phải ASCII

---

## 🛠️ Các bước xử lý dữ liệu
1. Load dữ liệu từ file CSV
2. Bổ sung header cho dataset
3. Làm sạch dữ liệu:
   - Xóa dòng trống
   - Xóa dữ liệu trùng lặp
   - Chuẩn hóa đơn vị cân nặng về **kgs**
4. Xử lý dữ liệu thiếu:
   - Thay thế giá trị thiếu Age bằng **mean**
   - Xóa dòng nếu thiếu cả Age và Weight
5. Chuyển đổi dữ liệu:
   - Melt các cột nhịp tim về dạng long format
   - Tách giới tính và khoảng thời gian
6. Xuất dữ liệu đã làm sạch ra file CSV

---

## 🚀 Cách chạy
1. Mở file notebook trong Google Colab:
2. Upload file `patient_heart_rate.csv` vào thư mục `data/`
3. Chạy toàn bộ notebook từ trên xuống dưới
4. File kết quả sẽ được lưu tại:
