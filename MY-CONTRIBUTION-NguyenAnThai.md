# Đóng góp cá nhân — Nguyễn An Thái

- Họ tên: **Nguyễn An Thái**
- MSSV: **2A20602159**
- Nhóm: **K4-DAY13-Nhom-LeDanhTrung**

## Công việc thực hiện

- Kiểm tra provenance của các output A/B/C, bảo đảm kết quả được thực hiện đúng theo pipeline và cấu hình đã quy định.
- Đối chiếu thông tin run, input, delta và pillar size để xác nhận các output tương ứng với đúng cấu hình A/B/C.
- Kiểm tra và phân tích các ca QC, đặc biệt là phân biệt lỗi ảnh hưởng toàn batch với lỗi cục bộ trên từng cuboid.
- Đối chiếu kết quả từ summary.csv, prediction JSON và ảnh Side để phát hiện các trường hợp bất thường trong prediction.
- Kiểm tra tính nhất quán giữa kết quả thực tế và nội dung được ghi trong PRE-LABEL-REPORT.md và TEAMMATES.md.
- Ghi nhận các vấn đề liên quan đến pipeline/frame transform, z-height và cuboid để nhóm có cơ sở xử lý hoặc báo cáo.
- Kiểm tra hồ sơ đóng góp cá nhân và các bằng chứng cần thiết trước khi nhóm hoàn thiện submission.

## Điều rút ra

Delta được áp dụng trước inference nên có thể thay đổi toàn bộ tập prediction, không chỉ dịch z của các hộp có sẵn. Pillar size thay đổi cách point cloud được gom thành biểu diễn đầu vào. Lỗi z đồng loạt cần kiểm pipeline; lỗi riêng một hộp cần kiểm theo đối tượng.

## Vai trò trong lượt chạy nhóm

Phạm Văn Thân trực tiếp vận hành runner. Lê Danh Trung kiểm tra output và tổng hợp báo cáo. Nguyễn An Thái kiểm provenance và các ca QC. Toàn nhóm sử dụng trạng thái `executed-by-group`.
