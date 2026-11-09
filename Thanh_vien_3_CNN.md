# CNN.ipynb — huy26ms23411@fsb.edu.vn
## Phụ trách: Kiến trúc CNN, compile, huấn luyện và đánh giá

**Phạm vi:** Cell 15–23; Mục 8–10.

### Các nội dung cần comment
1. **Xây dựng CNN từ đầu:** giải thích từng lớp Conv2D, activation, pooling, GlobalAveragePooling, Dropout và Dense; theo dõi kích thước tensor qua từng lớp.
2. **Compile và huấn luyện:**
   - Optimizer Adam, learning rate, binary cross-entropy.
   - Batch size, epoch, class weights.
   - Callback, early stopping và checkpoint nếu có.
   - Vì sao checkpoint được lựa chọn theo validation.
3. **Đọc kết quả huấn luyện:** giải thích train/validation loss và accuracy; nhận diện dấu hiệu overfitting hoặc underfitting mà không kết luận chỉ từ một đường biểu đồ.
4. **Đánh giá test:**
   - Vì sao test chỉ được dùng sau khi chốt mô hình.
   - Accuracy, balanced accuracy, precision, recall, F1, macro-F1 và ROC-AUC nếu được tính.
   - Confusion matrix và cách đọc lớp thật/dự đoán.
   - Ý nghĩa lớp dương là xe máy và ảnh hưởng mất cân bằng lớp.

### Câu hỏi cần tự trả lời
- Epoch và batch size là gì?
- Learning rate ảnh hưởng thế nào đến cập nhật trọng số?
- Vì sao dùng class weights?
- Precision và recall khác nhau thế nào?
- Khi dữ liệu mất cân bằng, vì sao accuracy có thể gây hiểu nhầm?
- Vì sao không chọn mô hình theo kết quả test?

### Đầu ra cần hoàn thành
Comment cell 15–23; có thể giải thích toàn bộ quy trình từ kiến trúc đến cập nhật trọng số và đánh giá định lượng.
