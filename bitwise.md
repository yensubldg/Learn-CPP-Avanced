# Lý thuyết

- Bản chất dữ liệu sẽ được máy tính lưu dưới dạng dãy các bit (dãy các con số 0 hoặc 1). Ví dụ:

```c++
char a = 4;
```

Biến `a` sẽ được máy tính lưu trữ bằng `8 bit` (kích thước kiểu `char` là `1 byte` mà `1 byte = 8 bit`) giống như sau:

```c++
0 0 0 0 0 1 0 1
```

- Các phép toán trên bit

1. Phép AND (&)

- Phép AND giữa 2 bit sẽ trả về 1 khi cả 2 bit đều có giá trị bằng 1, ngược lại nó sẽ trả về 0. Ví dụ:

```c++
0 & 0 = 0
0 & 1 = 0
1 & 0 = 0
1 & 1 = 1
```

2. Phép OR (|)

- Phép OR giữa 2 bit sẽ trả về 1 nếu có ít nhất 1 trong 2 bit có giá trị bằng 1, ngược lại nó sẽ trả về 0. Ví dụ:

```c++
0 | 0 = 0
0 | 1 = 1
1 | 0 = 1
1 | 1 = 1
```

3. Phép NOT (~)

- Phép NOT là phép đảo bit. Ví dụ:

```c++
~0 = 1
~1 = 0
```

4. Phép XOR (^)

- Phép XOR giữa 2 bit sẽ trả về 1 khi 2 bit có giá trị khác nhau, ngược lại nó sẽ trả về 0. Ví dụ:

```c++
0 ^ 0 = 0
0 ^ 1 = 1
1 ^ 0 = 1
1 ^ 1 = 0
```

5. Phép dịch trái (<<)

- Phép dịch trái là phép dịch tất cả các bit sang trái. Ví dụ:

```c++
A : 0 0 0 0 1 1 1 1
A << 2 : 0 0 1 1 1 1 0 0
```

6. Phép dịch phải (>>)

- Phép dịch phải là phép dịch tất cả các bit sang phải. Ví dụ:

```c++
A : 0 0 0 0 1 1 1 1
A >> 2 : 0 0 0 0 0 0 1 1
```
