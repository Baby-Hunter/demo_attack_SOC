# demo_attack_SOC
Dự án mô phỏng chuỗi hành vi tấn công trên hệ thống Linux, trong đó:

Kẻ tấn công sau khi có quyền truy cập vào máy mục tiêu sẽ tải và thực thi một script được lưu trữ trên GitHub.
Script thực hiện các hành vi mô phỏng malware, bao gồm:
-Download and Execute Payload: Tải và thực thi payload từ Internet. 
-Establish Persistence via systemd: Tạo user service nhằm duy trì khả năng thực thi tự động trên hệ thống.
-Establish Persistence via cron: Thiết lập cron job để tải và thực thi script từ xa định kỳ 5 phút một lần.
-Exfiltrate Sensitive Information: Gửi nội dung tệp /etc/passwd đến máy chủ bên ngoài thông qua HTTP POST.
-Collect Host Information: Thu thập thông tin hệ thống, bao gồm hostname, kernel và phiên bản hệ điều hành, sau đó gửi dữ liệu ra ngoài.
-Dự án phục vụ mục đích học tập, kiểm thử và xây dựng năng lực phát hiện, giám sát an ninh mạng (SOC).
