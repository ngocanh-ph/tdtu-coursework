# HUẤN LUYỆN MÔ HÌNH CƠ BẢN
## Bài toán: Phân loại hoa lan (Iris Classification)
Tập dữ liệu được lấy từ **UCI iris_dataset**
## 1.1 Mô tả bài toán
Một nhà thực vật học muốn phân loại hoa lan biết rằng mỗi bông hoa được mô tả bằng **4 đặc trưng**, bao gồm:
- Chiều dài cánh hoa (pedal length).
- Chiều rộng cánh hoa (petal width).
- Chiều dài lá đài (sepal length).
- Chiều rộng lá đài (sepal width).
Tất cả các đặc trưng đều được đo bằng **đơn vị cm**.  
Mỗi mẫu hoa được biểu diễn dưới dạng **một vector đặc trưng** với bốn thành phần tương ứng.
## 1.2 Dữ liệu
Nhà thực vật học sở hữu một tập dữ liệu gồm nhiều mẫu hoa lan đã được các chuyên gia phân loại trước đó.
Mỗi mẫu trong tập dữ liệu bao gồm:
- Một **vector đặc trưng (feature)** gồm bốn giá trị.
- Một **nhãn (label)** tương ứng với từng loài hoa.
Các mẫu được phân chia thành **ba lớp (class)** theo chủng loại:
- Setosa
- Versicolor
- Virginica
Mục tiêu bài toán là xây dựng **một mô hình học máy** có khả năng học từ dữ liệu đã gán nhãn, từ đó dự đoán chính xác **loài của một mẫu hoa mới chưa từng xuất hiện trong quá trình huấn luyện**.
## 1.3 Phân loại dạng bài toán
Dựa vào tập dữ liệu huấn luyện đã bao gồm **nhãn (label)** tương ứng cho từng mẫu, bài toán này thuộc vào nhóm **học có giám sát (Supervised Learning)**.
Bên cạnh đó, mô hình này có mục đích dự đoán **các giá trị rời rạc**, tức là giá trị khi dự đoán thuộc **một trong ba loại hoa lan** được xác định bởi chuyên gia cho trước. Vì vậy, đây là **một bài toán phân loại (Classification)**.
## 1.4 Quy trình thực hiện
Quá trình xây dựng mô hình phân loại được thực hiện theo các bước sau:
1. Khảo sát tập dữ liệu.
2. Chia dữ liệu thành tập **training** và **testing**.
3. Khảo sát đặc tính của dữ liệu.
4. Xây dựng và huấn luyện mô hình.
5. Thực hiện dự đoán trên tập dữ liệu mới.
6. Đánh giá mô hình.