# Cài đặt Node.js và Express.js

## Cài đặt Node.js

* Truy cập vào trang chủ [**Node.js**](https://nodejs.org/en)

* Chọn tải phiên bản LTS (Long term support)

* Tải về và cài đặt

* Kiểm tra **Node.js** và **npm** bằng lệnh `node -v` và `npm -v`. Nếu hiển thị kết quả phiên bản hiện tại tức là đã cài đặt thành công.

## Khởi tạo ứng dụng

Trước khi cài đặt Express.js, ta cần phải khởi tạo ứng dụng.

* Mở môi trường dòng lệnh (Terminal, Command Promt, ...). Nếu sử dụng [**Visual Studio Code**](https://code.visualstudio.com/download) thì có thể sử dụng **Terminal** có sẵn.

* Truy cập vào thư mục sẽ làm Workspace (chứa ứng dụng).

* Sử dụng lệnh `npm init` để khởi động ứng dụng. Các yêu cầu thông tin về ứng dụng sẽ lần lượt hiện ra. Nhập các thông tin hoặc ấn **Enter** để sử dụng giá trị mặc định được khuyến nghị.

> [!Note]
> Có thể sử dụng lệnh `npm init -y` để bỏ qua các câu hỏi về ứng dụng - sử dụng các giá trị mặc địnhh.


* Sau đó, file `package.json` được tạo ra với nội dung như sau (có thể khác biệt theo từng thông tin cung cấp):

```json
    {
        "name": "nodeapp",
        "version": "1.0.0",
        "description": "",
        "main": "index.js",
        "scripts": {
            "test": "echo \"Error: no test specified\" && exit 1"
        },
        "keywords": [
            "nodejs",
            "testnodejs"
        ],
        "author": "...",
        "license": "ISC"
    }
```

