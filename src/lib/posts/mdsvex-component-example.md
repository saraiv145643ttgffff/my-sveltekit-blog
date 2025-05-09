---
title: "Các khái niệm chính của hệ thống phân tán"
date: "2025-04-29"
updated: "2025-04-29"
categories:
  - "sveltekit"
  - "markdown"
  - "svelte"
coverImage: "/images/anh2.jpg"
coverWidth: 16
coverHeight: 9
excerpt: 
---

## 1. Scalability (Khả năng mở rộng)
- Khái niệm: Khả năng của hệ thống để xử lý sự gia tăng người dùng hoặc khối lượng công việc.
- Loại khả năng mở rộng:

 Mở rộng theo chiều dọc: Nâng cấp tài nguyên của một máy chủ duy nhất.
 Mở rộng theo chiều ngang: Thêm nhiều máy chủ vào hệ thống.
- Lợi ích: Đáp ứng nhu cầu hiện tại và chuẩn bị cho sự phát triển trong tương lai.
## 2. Fault Tolerance (Khả năng chịu lỗi)
- Khái niệm: Khả năng của hệ thống để tiếp tục hoạt động bình thường khi có sự cố.
- Kỹ thuật: Sử dụng sao chép dữ liệu và phân phối tải.
- Lợi ích: Đảm bảo dịch vụ không bị gián đoạn, đặc biệt trong các ứng dụng quan trọng.
## 3. Availability (Tính sẵn có)
- Khái niệm: Khả năng của hệ thống để đảm bảo rằng dịch vụ luôn sẵn có cho người dùng.
- Yếu tố ảnh hưởng: Thời gian ngừng hoạt động và khả năng phục hồi nhanh chóng.
- Lợi ích: Tăng cường lòng tin của người dùng vào dịch vụ.
## 4. Transparency (Tính minh bạch)
- Khái niệm: Người dùng không cần biết về các chi tiết bên trong của hệ thống.
- Yêu cầu: Hệ thống phải hoạt động như một đơn vị duy nhất.
- Lợi ích: Giảm bớt sự phức tạp cho người dùng và cải thiện trải nghiệm.
## 5. Concurrency (Đồng thời)
- Khái niệm: Khả năng của hệ thống để xử lý nhiều tác vụ cùng một lúc.
- Ứng dụng: Quan trọng trong các ứng dụng yêu cầu xử lý nhiều yêu cầu từ người dùng.
- Lợi ích: Đảm bảo hiệu suất cao trong thời gian thực.
## 6. Parallelism (Song song)
- Khái niệm: Khả năng của hệ thống để thực hiện nhiều tác vụ đồng thời.
- Sự khác biệt với đồng thời: Song song liên quan đến việc thực hiện nhiều tác vụ một cách thực tế.
- Lợi ích: Giảm thời gian xử lý trong các ứng dụng yêu cầu xử lý dữ liệu lớn.
## 7. Openness (Tính mở)
- Khái niệm: Khả năng của hệ thống để tích hợp với các hệ thống khác.
- Lợi ích: Cho phép mở rộng và cải thiện hệ thống dễ dàng.
- Ứng dụng: Tạo điều kiện cho việc phát triển các ứng dụng mới.
## 8. Vertical Scaling (Mở rộng theo chiều dọc)
- Khái niệm: Thêm tài nguyên vào một máy chủ duy nhất.
- Giới hạn: Có một điểm mà không thể nâng cấp thêm nữa.
- Thời gian ngừng hoạt động: Có thể xảy ra trong quá trình nâng cấp.
## 9. Horizontal Scaling (Mở rộng theo chiều ngang)
- Khái niệm: Thêm nhiều máy chủ vào hệ thống.
- Lợi ích: Tăng khả năng xử lý mà không gặp phải giới hạn.
- Tính linh hoạt: Dễ dàng mở rộng quy mô khi cần thiết.
## 10. Load Balancer (Bộ cân bằng tải)
- Khái niệm: Thiết bị hoặc phần mềm phân phối lưu lượng truy cập đến nhiều máy chủ.
- Lợi ích: Đảm bảo không có máy chủ nào bị quá tải.
- Cách hoạt động: Dựa trên địa chỉ IP, số lượng kết nối hoặc thời gian phản hồi.
## 11. Replication (Sao chép)
- Khái niệm: Tạo bản sao của dữ liệu trên nhiều máy chủ.
- Lợi ích: Tăng cường tính sẵn có và khả năng chịu lỗi.
- Phương pháp: Sao chép đồng bộ và không đồng bộ, tùy thuộc vào yêu cầu về độ chính xác và tốc độ.
## 12. Ví dụ và giải thích
## Ví dụ: Hệ thống thương mại điện tử
- Tình huống: Một trang web thương mại điện tử hoạt động trên kiến trúc phân tán.
- Khả năng mở rộng: Khi số lượng người dùng tăng, có thể thêm nhiều máy chủ để phục vụ lưu lượng truy cập.
- Khả năng chịu lỗi: Nếu một máy chủ gặp sự cố, các máy chủ khác vẫn có thể phục vụ người dùng.
- Tính sẵn có: Hệ thống luôn sẵn sàng 24/7 cho người dùng.
- Tính minh bạch: Người dùng không cần biết dữ liệu được lưu trữ ở đâu.
- Đồng thời: Nhiều người dùng có thể đặt hàng cùng lúc mà không gặp vấn đề.
- Song song: Các đơn hàng có thể được xử lý đồng thời trên nhiều máy chủ.
- Tính mở: Hệ thống có thể tích hợp với các dịch vụ thanh toán bên ngoài.
- Mở rộng theo chiều dọc: Có thể nâng cấp máy chủ hiện tại, nhưng có giới hạn.
- Mở rộng theo chiều ngang: Có thể thêm nhiều máy chủ mới để chia sẻ tải.
- Bộ cân bằng tải: Phân phối lưu lượng truy cập đến các máy chủ khác nhau.
- Sao chép: Dữ liệu khách hàng được sao chép trên nhiều máy chủ để đảm bảo tính sẵn có.