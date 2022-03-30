# Kiểu cấu trúc (struct)

- Kiểu struct cho phép bạn kết hợp các kiểu dữ liệu lại thành 1 kiểu dữ liệu mới do bạn tự định nghĩa.

Ví dụ nếu bạn cần viết chương trình lưu thông tin về tên và tuổi của 100 sinh viên, với cách làm thông thường bạn sẽ tạo ra 2 mảng giống như sau:

```c++
string names[100];
int ages[100];
```

Với `struct` thì bạn sẽ định nghĩa kiểu dữ liệu `Student` với 2 thuộc tính là `name` và `age` giống như sau:

```c++
struct Student {
    string name;
    int age;
};
```

và bây giờ thay vì dùng 2 mảng `names` và `ages` thì bạn dùng mảng các đối tượng `Student`

```c++
Student students[100];
```

Có thể thấy viết `Student students[100];` sẽ rõ nghĩa hơn là viết 2 mảng `names` và `ages`. Hơn nữa với cách làm cũ nếu chương trình của bạn cần lưu trữ 10 thuộc tính của học sinh thì bạn phải tạo ra 10 mảng và nếu có truyền thông tin học sinh vào hàm thì hàm phải có 10 tham số đầu vào. Còn với `struct` thì bạn chỉ cần truyền vào hàm 1 tham số.

Để truy xuất vào các thuộc tính của một đối tượng kiểu struct bạn có thể gọi `tên_đối_tượng.tên_thuộc_tính`. Ví dụ:

```c++
#include<iostream>

using namespace std;

// Khai báo struct student với 2 thuộc tính là name và age
struct Student {
	string name;
	int age;
};

int main() {
	// Tạo ra 1 đối tượng kiểu Student để lưu thông tin của 1 sinh viên
	Student s1;
	s1.name = "Blackcat";
	s1.age = 24;
	cout << "Name: " << s1.name << endl;
	cout << "Age :" << s1.age;
	return 0;
}
```

Kết quả khi chạy chương trình:

```
Name: Blackcat
Age :24
```
