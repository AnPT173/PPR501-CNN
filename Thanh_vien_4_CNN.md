# CNN.ipynb — Thành viên 4
## Phụ trách: Phân tích dự đoán, feature map, lưu và kết luận

**Phạm vi:** Cell 24–32; Mục 11–14.1.

### Các nội dung cần comment
1. **Xem dự đoán và ảnh sai:**
   - Giải thích cách hiển thị ảnh, nhãn thật, nhãn dự đoán và xác suất.
   - Phân tích các trường hợp nhầm lẫn; nêu các yếu tố có thể liên quan như góc chụp, nền, màu sắc, che khuất.
   - Phân biệt quan sát được với giả thuyết về nguyên nhân.
2. **Quan sát feature map:**
   - Cách lấy activation từ các lớp convolution.
   - Mỗi feature map thể hiện phản hồi của một filter.
   - Giới hạn: feature map không tự chứng minh mô hình dựa vào vùng/đặc trưng nào để ra quyết định.
3. **Lưu mô hình và dự đoán ảnh riêng:**
   - Nội dung file `.keras` và JSON cấu hình.
   - Hàm nạp mô hình, preprocessing ảnh riêng và ánh xạ thứ tự nhãn.
   - Vì sao preprocessing inference phải khớp với preprocessing lúc train.
4. **Tổng hợp và kết luận:**
   - Phân biệt số liệu thực nghiệm với nhận xét.
   - Nêu giới hạn dữ liệu Caltech-101, số lớp, kích thước dữ liệu và khả năng tổng quát.
   - Không tuyên bố mô hình nhận dạng tốt trong cảnh giao thông thực tế nếu chưa kiểm thử độc lập.

### Câu hỏi cần tự trả lời
- Vì sao cần phân tích ảnh dự đoán sai?
- Feature map cho biết điều gì và không chứng minh được điều gì?
- Vì sao cần lưu cấu hình và thứ tự nhãn cùng mô hình?
- Nếu preprocessing inference khác train thì có thể xảy ra điều gì?
- Giới hạn lớn nhất của thực nghiệm CNN là gì?

### Đầu ra cần hoàn thành
Comment cell 24–32 và chuẩn bị phần trình bày kết quả, hạn chế, hướng cải thiện.
