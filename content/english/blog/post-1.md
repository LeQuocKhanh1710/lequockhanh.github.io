---
title: "Nghiên cứu về Malware trong QR code"
meta_title: "Phân tích và phòng chống tấn công Malware lây lan qua Mã QR"
description: "Bài nghiên cứu chuyên sâu về các phương thức mà tội phạm mạng sử dụng QR Code để phân tán phần mềm độc hại, từ QRishing đến nhúng mã độc trực tiếp."
date: 2025-08-04T05:00:00Z
image: "/images/QR.png"
categories: ["Software", "Technology", "Cybersecurity"] # Thêm Cybersecurity nếu phù hợp
author: "Lê Quốc Khánh"
tags: ["Malware", "QR Code", "Security", "Cybersecurity", "Phishing"] # Thêm tags cụ thể hơn
draft: false
---

Trong kỷ nguyên số, Mã QR (QR Code) đã trở thành một công cụ tiện lợi cho mọi giao dịch, từ thanh toán di động đến chia sẻ thông tin. Tuy nhiên, sự tiện lợi này cũng mở ra một cánh cửa mới cho các mối đe dọa an ninh mạng. Bài nghiên cứu này đi sâu vào cách thức các phần mềm độc hại (Malware) đang được phân tán tinh vi thông qua QR Code.

### Mối đe dọa QRishing và Tấn công Redirection

Hình thức tấn công phổ biến nhất liên quan đến QR Code là **QRishing** (kết hợp QR và Phishing). Kẻ tấn công tạo ra các mã QR giả mạo, dán đè lên mã QR hợp pháp ở nơi công cộng. Khi người dùng quét mã, họ bị chuyển hướng (redirection) đến một trang web lừa đảo.

> Mục tiêu chính của QRishing là đánh cắp thông tin đăng nhập, tài khoản ngân hàng hoặc buộc nạn nhân tải xuống một tệp tin chứa mã độc (dropper).

### Phân loại các kiểu Malware lây nhiễm qua QR Code

Các Malware được phân phối qua phương thức này có thể đa dạng, tùy thuộc vào mục tiêu của kẻ tấn công:

#### 1. Dropper và Downloader
Các mã QR chứa liên kết trực tiếp đến một tệp `.apk` hoặc `.exe` nhỏ. Sau khi được tải về, tệp này sẽ tự động tải xuống và cài đặt Malware lớn hơn (như Ransomware hoặc Trojan) vào thiết bị của nạn nhân.

#### 2. Mã độc nhúng vào Ứng dụng Quét
Một số trường hợp hiếm hơn, kẻ tấn công phát triển các ứng dụng quét QR Code giả mạo. Các ứng dụng này tự nó đã là Spyware, âm thầm thu thập dữ liệu người dùng ngay từ khi được cài đặt.

### Biện pháp Phòng chống và Nhận diện

Để tự bảo vệ mình khỏi các nguy cơ tiềm tàng từ QR Code Malware, người dùng cần tuân thủ các nguyên tắc bảo mật cơ bản:

1.  **Kiểm tra vật lý:** Luôn kiểm tra xem mã QR có bị dán đè hay thay thế ở nơi công cộng không.
2.  **Xem trước URL:** Sử dụng các ứng dụng quét QR Code có tính năng xem trước (preview) URL trước khi truy cập.
3.  **Không tải tệp lạ:** Tuyệt đối không tải xuống và cài đặt các tệp tin lạ (APK, EXE) từ các trang web không đáng tin cậy.

Phòng chống là ưu tiên hàng đầu, vì việc loại bỏ Malware sau khi đã bị lây nhiễm thường rất phức tạp và tốn kém.