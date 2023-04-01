# wirte-up_CTF
Đầu tiên thì đây là link đề: https://play.picoctf.org/practice/challenge/350?category=4&originalEvent=72&page=1.
nhấn vào rồi tải ảnh về:![flag](https://user-images.githubusercontent.com/118189974/229268509-2df001c0-794c-4c90-918e-f21032a6a490.png)

thấy ngay ở trên đề bài có yêu cầu steganography(Kỹ thuật giấu tin).
lên google search steganography decode(sẽ như này):
![image](https://user-images.githubusercontent.com/118189974/229268568-ce855a0a-bca1-4ab2-8541-d8d423c112b7.png)
chọn decode rồi tải ảnh lên, ấn decode sẽ ra được Hidden message...rồi tìm từ khóa picoCTF
nhưng không có => không được mã hóa bằng kiểu text.
còn 1 kiểu mã hóa steghide.
Kho lưu trữ zip được giải nén bằng binwalk :
$ binwalk -e flag.png
Điều này mang lại một flag.png khác trong hideme/_flag.png.extracted/secret/flag.png mà khi được xem bằng trình chỉnh sửa hình ảnh và hiển thị flag:
                                        dạng: picoCTF{........XXXXXX........}
