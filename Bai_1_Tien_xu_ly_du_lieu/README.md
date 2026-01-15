# Bài 1: Tiền xử lý và thao tác dữ liệu tuyển sinh đại học

## 1. Mục tiêu
- Làm quen với thao tác dữ liệu bằng Pandas
- Xử lý dữ liệu thiếu
- Chuẩn hóa và chuyển đổi dữ liệu
- Tạo biến mới phục vụ phân tích
- Phân loại học lực và xác định kết quả xét tuyển

## 2. Công nghệ sử dụng
- Python 3
- Google Colab
- Pandas
- NumPy

## 3. Dữ liệu
- File gốc: `dulieuxettuyendaihoc.csv`
- File sau xử lý: `processed_dulieuxettuyendaihoc.csv`

## 4. Cách hoạt động
1. Đọc dữ liệu từ file CSV
2. Phân loại biến định tính và định lượng
3. Xử lý dữ liệu thiếu:
   - Cột dân tộc (DT): điền giá trị 0
   - Các cột điểm: thay thế bằng giá trị trung bình (Mean)
4. Tạo các biến trung bình môn:
   - TBM1 (lớp 10)
   - TBM2 (lớp 11)
   - TBM3 (lớp 12)
5. Xếp loại học lực:
   - Y: Yếu
   - TB: Trung Bình
   - K: Khá
   - G: Giỏi
   - XS: Xuất sắc
6. Chuẩn hóa điểm trung bình sang thang điểm 4 (US_TBM)
7. Xác định kết quả xét tuyển đại học (KQXT)

## 5. Kết quả
- Dataset đã được làm sạch và xử lý
- Notebook `lab1.ipynb` thể hiện đầy đủ các bước xử lý dữ liệu
- File kết quả sẵn sàng cho các bước phân tích tiếp theo
