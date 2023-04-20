# Tab, Tab, Attack


link : https://play.picoctf.org/practice/challenge/176?category=5&page=

# đầu tiên, coppy địa chỉ liên kết ở phần tải file: http://mercury.picoctf.net/static/72712e82413e78aa8d53ffea42b0/Addadshashhanammu.zip
mở kali:


# dùng lệnh : wget http://mercury.picoctf.net/static/72712e82413e78aa8d53ffea42b0/Addadshashhanammu.zip 


sau đó  dùng kiểm tra dùng : ls.


# dùng lệnh : grep "pico" -r Addadshashanammu

<Với lệnh này, grep sẽ tìm kiếm tất cả các tệp tin trong thư mục Addadshashanammu (bao gồm các tệp tin trong các thư mục con) và hiển thị các dòng chứa chuỗi "pico>

=>Thông báo lỗi: 

"grep: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/fang-of-haynekhtnamet: binary file matches".

có nghĩa là lệnh grep không thể tìm kiếm được chuỗi trong tệp tin fang-of-haynekhtnamet, bởi vì đó là một tệp nhị phân (binary file).

do đó sử dụng: 
# strings fang-of-haynekhtnamet | grep "pico"



=> flag : picoCTF{l3v3l_up!_t4k3_4_r35t!_6f332f10}
