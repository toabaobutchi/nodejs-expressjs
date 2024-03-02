# Cài đặt Node.js và Express.js

## Cài đặt Node.js

* Truy cập vào trang chủ [**Node.js**](https://nodejs.org/en)

* Chọn tải phiên bản LTS (Long term support)

* Tải về và cài đặt

* Kiểm tra **Node.js** và **npm** bằng lệnh `node -v` (hoặc `node --version`) và `npm -v` (hoặc `npm --version`). Nếu hiển thị kết quả phiên bản hiện tại tức là đã cài đặt thành công.

## Khởi tạo ứng dụng

Trước khi cài đặt Express.js, ta cần phải khởi tạo ứng dụng.

* Mở môi trường dòng lệnh (Terminal, Command Promt, ...). Nếu sử dụng [**Visual Studio Code**](https://code.visualstudio.com/download) thì có thể sử dụng **Intergrated Terminal** có sẵn.

* Truy cập vào thư mục sẽ làm Workspace (chứa ứng dụng).

* Sử dụng lệnh `npm init` để khởi động ứng dụng. Các yêu cầu thông tin về ứng dụng sẽ lần lượt hiện ra. Nhập các thông tin hoặc ấn **Enter** để sử dụng giá trị mặc định được khuyến nghị.

> [!Note]
> Có thể sử dụng lệnh `npm init -y` để bỏ qua các câu hỏi về ứng dụng và sử dụng các giá trị mặc địnhh.


* Sau đó, file `package.json` được tạo ra với nội dung như sau (có thể khác tuỳ vào thông tin cung cấp):

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

## Cài đặt Express.js

Cài đặt Express.js thông qua npm bằng lệnh sau:

```sh
npm install express
# hoặc
npm i express
```

Nếu sử dụng npm phiên bản 4 hoặc thấp hơn, hãy thêm cờ `--save` trong câu lệnh cài đặt.

Sau khi cài đặt Express.js, thư mục `node_modules` và `package-lock.json` được tạo ra nhằm khai báo và chứa các thư viện cần thiết.
