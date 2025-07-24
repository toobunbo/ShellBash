# Shell Bash
Với cá nhân mình thì việc học một ngôn ngữ mới đơn giản chỉ là học syntax ~~Hoặc Không 😃~~
### Khác biệt giữa Scripting Language và Programing Lang
Ừ thì Bash là một Scripting Language dùng để giao tiếp với hệ điều hành dựa trên Unix và đưa ra lệnh cho hệ thống. Vậy khác gì so với các Programing Lan như Java, C++, ...
Tự tìm hiểu đi hẹ hẹ
## Cấu trúc của một Shell Bash
Cơ bản thì sẽ gồm có:
- Shebang
- if-else-fi
- Khai báo biến
- echo (print)
- Special Variable
<code>
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

### Shebang
Shebang luôn là dòng đầu tiên của script, bắt đầu bằng "#!/path". Dòng này chỉ định đường dẫn thông dịch mà tệp thực thi, ví dụ:
- Python: #!/usr/bin/env python
- Perl: #!/usr/bin/env perl
*Hơi khó hiểu nhưng mà hiểu được về Scripting và Progarming Lan thì hiểu được thôi, không giải thích nhiều* ~~ngu~~

## Conditional Excution
Không nói nhiều về if-else-fi, while,... Tự tìm hiểu cái này cũng như các toán tử đi. ~~hint: Toán tử về kiểm tra file khá hay~~:
- string Operators
- interger Operators
- boolean Operators
- file Operators


<img width="1346" height="986" alt="image" src="https://github.com/user-attachments/assets/b5396691-dfd6-49bc-b331-8c0c520254ab" />

## Arguments, Variables, and Arrays
### Arguments
Có thể truyền tối đa 9 Arguments `bash test.sh ARG1 ARG2 ... ARG9`. *Vậy $0 cho ta biết về gì ?*

### Variables
Làm biếng viết quá để cái demo ở đây mai viết tiếp.
- Code:
<code>
#!/bin/bash

echo "Count Parameter: $#"
echo "Test \"\$@"":"
for arg in "$@"
do
        echo " - Tham số: $arg"
done

echo "Test \"\$*"":"
for arg in "$*"
do
        echo " - Tham số: $arg"
done
</code>

- Thực thi:
  <img width="1082" height="196" alt="image" src="https://github.com/user-attachments/assets/ed415c78-3122-4681-8951-7b094709896d" />






