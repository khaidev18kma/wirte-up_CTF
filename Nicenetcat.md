Tổng quát: Đầu tiên, kết nối mercury.picoctf.net 43239 trong Linux terminal.
nhận được các số hexa:
112 105 99 111 67 84 70 123 103 48 
48 100 95 107 49 116 116 121 33 95 
110 49 99 51 95 107 49 116 116 121 
33 95 55 99 48 56 50 49 102 53 125 10
viết mã C đơn giải:
#include <stdio.h>
#define max 1000
int main(){
	int a[max] = {112, 105, 99, 111, 67, 84, 70, 123, 103, 48,
			 48, 100, 95, 107, 49, 116, 116, 121, 33, 95,
			110, 49, 99, 51, 95, 107, 49, 116, 116, 121, 
			33, 95, 55, 99, 48, 56, 50, 49, 102, 53, 125, 10};
	for(int i = 0; i < 42; i++){
		printf("%c", a[i]);
	}
}
=> flag : picoCTF{g00d_k1tty!_n1c3_k1tty!_7c0821f5}

