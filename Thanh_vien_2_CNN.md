# CNN.ipynb — Thành viên 2
## Phụ trách: Đọc dữ liệu, chia tập và tiền xử lý

**Phạm vi:** Cell 8–14; Mục 5–7.

### Các nội dung cần comment
1. **Đọc, kiểm tra và loại ảnh trùng:**
   - Luồng ảnh bytes → mở ảnh → sửa hướng EXIF → RGB → resize có đệm.
   - Cách xử lý ảnh lỗi và cách ghi nhận ảnh bị loại.
   - Hash của ma trận RGB sau preprocessing; giới hạn của cách phát hiện ảnh trùng chính xác.
   - Nhận xét nguy cơ thiên lệch dữ liệu: khác biệt màu sắc/nền giữa hai lớp.
2. **Chia train/validation/test:**
   - Vai trò của từng tập.
   - Vì sao dùng stratified split và seed cố định.
   - Ý nghĩa kiểm tra rò rỉ giữa các tập.
   - Vì sao không dùng test để lựa chọn cấu hình hoặc checkpoint.
3. **Augmentation và chuẩn hóa:**
   - Giải thích từng phép biến đổi được dùng.
   - Vì sao augmentation chỉ áp dụng trong huấn luyện.
   - Vì sao chuẩn hóa pixel và giữ cùng preprocessing khi đánh giá/suy luận.
   - Nêu rõ các biến/hàm trả về và shape dữ liệu.

### Câu hỏi cần tự trả lời
- Vì sao phải kiểm tra ảnh trùng trước khi chia tập?
- Validation khác test như thế nào?
- Stratified split giải quyết vấn đề gì?
- Vì sao không augmentation trên test?
- Resize có giữ tỉ lệ và thêm padding khác gì kéo giãn ảnh?

### Đầu ra cần hoàn thành
Comment đầy đủ cell 8–14, đặc biệt là đầu vào/đầu ra của từng hàm và shape của `X`, `y` ở các giai đoạn.
