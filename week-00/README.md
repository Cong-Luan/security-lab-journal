## Đánh giá phần cứng
| Thành phần | Kết luận |
|---|---|
| CPU Core Ultra 5 225U, 12C/14T | Đủ. Chip U tiết kiệm điện nên chạy lâu sẽ nóng và tụt xung. Cắm sạc, để chế độ Best Performance khi chạy lab |
| RAM 32GB | Đủ cho lab tháng 2 (khoảng 5 VM). Tháng 4 (SIEM) phải tắt bớt VM. Khi chạy lab không mở Chrome 40 tab |
| SSD 512GB, trống 164GB | **Điểm yếu.** Thấp hơn mức 250GB đã yêu cầu. Phải dùng thin disk, xóa snapshot cũ. Trước tháng 4 phải có SSD ngoài USB-C 1TB, hoặc dọn ổ C xuống còn trống 250GB |
| Chỉ có Wi-Fi AX211 | Bridged qua Wi-Fi chập chờn. Lab dùng **NAT + Host-only/LAN Segment**, không dùng bridged |
| Đã có WSL2 + VMware | WSL2 bật Hyper-V. VirtualBox chạy chung với Hyper-V sẽ chậm và lỗi. **Chốt dùng VMware Workstation Pro** (miễn phí cho cá nhân), bỏ VirtualBox |

## Câu hỏi vặn
- Card NAT và host-only khác nhau là NAT cho kết nối với bên ngoài còn host-only chỉ cho kết nối mạng nội bộ.
- Không dùng bridge trên wifi vì ok ổn định về mạng dễ xung đột.
- Khi commit đã push mà dùng --amend sẽ làm thay đổi nội dung của lần commit đó.

