# Writeup-BabyRecon
Writeup CTF Baby Recon. Một thử thách tìm kiếm thông tin liên quan đến một Website, link dẫn đến thử thách: https://ctf.viblo.asia/puzzles/baby-recon-rhsybhqdrvi

# Đề bài
<img width="614" alt="image" src="https://github.com/user-attachments/assets/b7efe23f-79a4-4727-852a-9316ff48c3ad" />

# Phân tích 
Đầu tiên chúng ta tải về file favicon.zip được đính kèm đề bài. Giải nén & mở ảnh lên sẽ là một biểu tượng lạ mắt.

<img width="261" alt="image" src="https://github.com/user-attachments/assets/b6fdbf0d-2b8d-427c-b1b3-294ba00eb33c" />

Để tìm thêm thông tin liên quan đến bức ảnh này, chúng ta sẽ thực hiện sử dụng một tính năng sẵn có của Google đó là tìm kiếm bằng hình ảnh. Sau khi thực hiện, ở kết quả đầu tiên của kết quả tìm kiếm sẽ là Website đang sử dụng bức ảnh này. Chúng ta click vào để truy cập đến Website.

<img width="676" alt="image" src="https://github.com/user-attachments/assets/8ef8aee7-30de-47fd-a620-a22e10f09749" />

<img width="959" alt="image" src="https://github.com/user-attachments/assets/9a1a8a7f-30a4-421e-bebf-89a1989e7361" />


Để tìm kiếm được thông tin của quốc gia nơi đặt máy chủ host của một Website, chúng ta có khá nhiều cách. Đơn giản nhất sẽ là đi tìm các thông tin liên quan của một tên miền, để thực hiện điều này, chúng ta có thể sử dụng nhiều cách thức bao gồm tra cứu thông tin về tên miền tại các Website chuyên cung cấp dịch vụ hosting. Thực hiện tìm kiếm các thông tin liên quan đến tên miền "Viblo.asia", chúng ta thu thập được các thông tin sau: 

<img width="432" alt="image" src="https://github.com/user-attachments/assets/f080fe33-02d1-4804-9f31-29f0a5822466" />
<img width="418" alt="image" src="https://github.com/user-attachments/assets/9de17e10-b118-4774-9b57-9a233e3794f9" />
<img width="422" alt="image" src="https://github.com/user-attachments/assets/fa166ae5-b0bc-4157-8bc6-bae839668f30" />


+ Cloud Provider của Website có thể là Cloudflare
+ Các thông tin liên quan đến đăng ký của Website chủ yếu là tại Nhật Bản
+ Thông tin "Registrant Country" là "JP", vì vậy có thể khẳng định Website này được host tại Nhật Bản.
