# Shell Bash
Với cá nhân mình thì việc học một ngôn ngữ mới đơn giản chỉ là học syntax ~~Hoặc Không 😃~~
### Khác biệt giữa Scripting Language và Programing Lang
Ừ thì Bash là một Scripting Language dùng để giao tiếp với hệ điều hành dựa trên Unix và đưa ra lệnh cho hệ thống. Vậy khác gì so với các Programing Lan như Java, Python, C++, ...
Tự tìm hiểu đi hẹ hẹ
## Cấu trúc của một Shell Bash
Cơ bản thì sẽ gồm có:
- Shebang
- if-else-fi
- Khai báo biến
- echo (print)
- Special Variable

<code> <h2> Code mẫu
#!/bin/bash
# Check for given argument
if [ $# -eq 0 ]
then
	echo -e "You need to specify the target domain.\n"
	echo -e "Usage:"
	echo -e "\t$0 <domain>"
	exit 1
else
	domain=$1
fi 
</code>

## Conditional Excution



