# CNN.ipynb — Thành viên 1
## Phụ trách: Giới thiệu bài toán, lý thuyết CNN và dữ liệu

**Phạm vi:** Cell 0–7; Mục 1–4.

### Các nội dung cần comment
1. **Mục tiêu và cách chạy:** giải thích bài toán phân loại một ảnh thành ô tô hoặc xe máy; nêu môi trường, thư viện, backend Keras 3/PyTorch và seed.
2. **Phát biểu bài toán:** giải thích ảnh RGB đầu vào, xác suất sigmoid đầu ra, quy ước nhãn 0 = ô tô, 1 = xe máy, ngưỡng 0,5 và lớp dương.
3. **Cơ sở lý thuyết CNN:**
   - Kernel/filter trượt trên ảnh và dùng chung trọng số.
   - Feature map, convolution/cross-correlation, stride, padding và kích thước đầu ra.
   - ReLU, MaxPooling, GlobalAveragePooling, Dropout, Sigmoid.
   - Binary cross-entropy và vai trò của Adam.
4. **Ví dụ phép tính tay:** giải thích patch, kernel, phép nhân từng phần tử, tổng, ReLU và MaxPooling; nhấn mạnh kernel ví dụ không phải filter đã học.
5. **Nguồn dữ liệu/cấu hình:** hai nhóm `car_side` và `Motorbikes` của Caltech-101; lý do resize về 64×64 RGB; các hằng số cấu hình.

### Câu hỏi cần tự trả lời
- CNN khác mạng fully-connected ở điểm nào khi xử lý ảnh?
- Kernel và feature map là gì?
- Vì sao cần ReLU và pooling?
- Sigmoid trả về gì? Vì sao dùng binary cross-entropy?
- Vì sao ví dụ kernel tính tay không thể xem là filter mô hình đã học?

### Đầu ra cần hoàn thành
Comment các cell 0–7 theo từng khối logic; có thể trình bày từ bài toán, dữ liệu đến nguyên lý CNN mà không đọc lại code.
