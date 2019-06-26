
## Markdown

### Mục lục

[I. Ngôn ngữ Markdown](#ngonngumarkdown)
- [1. Thẻ tiêu đề](#thetieude)
- [2. Chèn link, chèn ảnh](#chenlinkchenanh)
- [3. Ký tự in đậm, in nghiêng](#kytuindaminnghieng)
- [4. Trích dẫn, bo chữ](#trichdanbochu)
- [5. Gạch đầu dòng](#gachdaudong)
- [6. Danh sách](#danhsach)
- [7. Tạo bảng](#taobang)
- [Mẹo](#meo)
	
===========================

## II. Ngôn ngữ Markdown

Markdown là ngôn ngữ đánh dấu văn bản được tạo ra bởi [John Gruber](https://en.wikipedia.org/wiki/John_Gruber). Markdown cho phép bạn viết bằng cách sử dụng định dạng văn bản đơn giản dễ đọc, dễ viết, sau đó chuyển đổi nó thành HTML có cấu trúc hợp lệ. Ngược lại các văn bản được viết bằng HTML cũng có thể được chuyển đổi sang Markdown.


### 1. Thẻ tiêu đề

Markdown sử dụng kí tự # để bắt đầu cho các thẻ tiêu đề. Các lớp tiêu đề h1, h2, h3 cho đến h6 có thể viết được bằng cách thêm số lượng ký tự # tương ứng vào đầu dòng. Một ký tự # tương đương với h1, 2 ký tự # tương đương với h2 ... Mức độ riêu đề giảm dần từ 1 đến 6.

Ví dụ:

```
# 1.Tiêu đề cấp 1
```

# 1.Tiêu đề cấp 1

```
## 2.Tiêu đề cấp 2
```

## 2.Tiêu đề cấp 2

```
###### 6.Tiêu đề cấp 6
```

###### 6.Tiêu đề cấp 6

### 2. Chèn link, chèn ảnh

Để chèn hyperlink bạn chỉ cần paste link đó vào file .md

```
đường dẫn
```

đường dẫn

Hoặc bạn cũng có thể sử dụng cú pháp sau để thu ngắn đường dẫn của link

```
[tên đường dẫn](đường dẫn)
```

Kết quả là:

[tên đường dẫn](đường dẫn)

Để chèn ảnh thì bạn hãy sử dụng cú pháp sau:

```
<img src="đường dẫn link ảnh">
```

Bạn có thể sử dụng công cụ [Lightshot](https://app.prntscr.com/en/index.html) để chụp ảnh màn hình và up hình đó lên trang [Imgur](https://imgur.com/) rồi lấy đường dẫn ảnh đưa vào Github

Hai công cụ này khá dễ sử dụng, bạn chỉ cần chụp màn hình bằng Lightshot ấn Ctrl + C để copy và Ctrl + V để paste vào trình duyệt tại trang web [Imgur](https://imgur.com/)

### 3. Ký tự in đậm, in nghiêng

- Để in đậm ký tự, bạn chỉ cần làm như sau:

```
**từ cần in đậm**
```

kết quả:

**từ cần in đậm**

- Để in nghiêng ký tự, bạn chỉ cần làm như sau:

```
*từ cần in nghiêng*
```

kết quả:

*từ cần in nghiêng*


### 4. Trích dẫn, bo chữ

Để bo một đoạn text thì bạn chỉ cần sử dụng cú pháp sau:

```
`đoạn cần bo`
```

Kết quả là: `đoạn cần bo`

Để làm nổi bật một đoạn văn, chẳng hạn như một đoạn code hay file cấu hình bạn có thể sử dụng cú pháp như sau:

    ```sh
    auto eth0
    iface eth0 inet static
    ipaddress 10.10.10.10
	netmask 255.255.255.0
	gateway 10.10.10.1
	dns-nameservers 8.8.8.8
    ```

Kết quả như sau:

```sh
auto eth0
iface eth0 inet static
ipaddress 10.10.10.10
netmask 255.255.255.0
gateway 10.10.10.1
dns-nameservers 8.8.8.8
```

### 5. Gạch đầu dòng

Để sử dụng gạch đầu dòng bạn chỉ cần sử dụng cú pháp sau:

```
- Gạch đầu dòng thứ nhất
  
  - Thụt với đầu dòng 1
  
  - Thụt với đầu dòng 1
 
- Gạch đầu dòng thứ hai
  
  - Thụt với đầu dòng 2
  
  - Thụt với đầu dòng 2
  
```

- Gạch đầu dòng thứ nhất
  
  - Thụt với đầu dòng 1
  
  - Thụt với đầu dòng 1
  
- Gạch đầu dòng thứ hai
  
  - Thụt với đầu dòng 2
  
  - Thụt với đầu dòng 2
  
### 6. Danh sách

Markdown hỗ trợ các danh sách được sắp xếp (đánh số) và không có thứ tự (gạch đầu dòng).

Danh sách không có thứ tự sử dụng dấu hoa thị, dấu cộng và dấu gạch nối - có thể thay thế cho nhau:

```
- Một
- Hai
- Ba
```

hoặc:

```
+ Một
+ Hai
+ Ba
```

hoặc:

```
* Một
* Hai
* Ba
```

kết quả:

- Một
- Hai
- Ba


### 7. Tạo bảng

Bạn có thể sử dụng cú pháp sau để tạo bảng:

```
| Cột 1 Hàng 1 | Cột 2 | Cột 3| Cột 4 |
|--------------|-------|------|-------|
| Hàng 2 | 2 x 1 | 2 x 2 | 2 x 3 | 2 x 4 |
| Hàng 3 | 3 x 1 | 3 x 2 | 3 x 3 | 3 x 4 |
| Hàng 4 | 4 x 1 | 4 x 2 | 4 x 3 | 4 x 4 |
```

Kết quả:

| Cột 1 Hàng 1 | Cột 2 | Cột 3| Cột 4 |
|--------------|-------|------|-------|
| Hàng 2 | 2 x 1 | 2 x 2 | 2 x 3 | 2 x 4 |
| Hàng 3 | 3 x 1 | 3 x 2 | 3 x 3 | 3 x 4 |
| Hàng 4 | 4 x 1 | 4 x 2 | 4 x 3 | 4 x 4 |

<a name="meo"></a>
###*Mẹo:*

- Sử dụng trang [Markdown Line Preview](https://markdownlivepreview.com/) paste vào đó đoạn markdown bạn viết và xem trước để chỉnh sửa cho phù hợp.

- Bạn cũng có thể sử dụng những đoạn markdown của người khác đã viết trước để tham khảo.
