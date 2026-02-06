 Titanic Disaster Analysis

 1. Giới thiệu

Bài thực hành phân tích dữ liệu Titanic nhằm mục tiêu:
- Làm sạch dữ liệu (Data Cleaning)
- Xây dựng đặc trưng mới (Feature Engineering)
- Phân tích khám phá dữ liệu (EDA)
- Trực quan hóa các yếu tố ảnh hưởng đến khả năng sống sót

Dữ liệu sử dụng: `titanic_disaster.csv`

---

 2. Thư viện sử dụng

- pandas
- numpy
- seaborn
- matplotlib

---

 3. Tiền xử lý dữ liệu

Các bước xử lý chính:

- Kiểm tra và xử lý dữ liệu thiếu
- Thay thế giá trị thiếu của Age theo trung bình từng Pclass
- Tạo biến Agegroup (Kid, Teen, Adult, Older)
- Tạo biến familySize = 1 + SibSp + Parch
- Rút gọn giới tính: male → M, female → F
- Trích xuất typeCabin từ Cabin
- Tách Name thành firstName và secondName

---

 4. Phân tích khám phá dữ liệu (EDA)

 4.1 Sống sót theo giới tính
- Nữ có tỷ lệ sống sót cao hơn nam.
- Giới tính là yếu tố ảnh hưởng mạnh.

 4.2 Sống sót theo hạng vé (Pclass)
- Hạng 1 có tỷ lệ sống cao nhất.
- Hạng 3 có tỷ lệ tử vong cao.

 4.3 Sống sót theo giới tính và độ tuổi
- Trẻ em và phụ nữ được ưu tiên cứu.
- Nam trưởng thành tử vong nhiều nhất.

 4.4 Sống sót theo số người đi cùng
- Nhóm gia đình nhỏ (2–4 người) có tỷ lệ sống cao hơn.
- Đi một mình có tỷ lệ sống thấp.

 4.5 Sống sót theo giá vé
- Giá vé cao tương ứng với khả năng sống sót cao.
- Fare liên quan đến Pclass.

 4.6 Sống sót theo Pclass và cảng lên tàu
- Hạng 3 tại cảng S có số tử vong cao nhất.
- Hạng 1 có tỷ lệ sống cao ở hầu hết các cảng.

---

 5. Kết luận

Các yếu tố ảnh hưởng mạnh nhất đến khả năng sống sót:

- Giớ
