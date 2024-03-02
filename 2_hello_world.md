# Hello World trong Express.js

Tại thư mục làm việc hiện tại, tạo một file `*.js` và sao chép đoạn mã bên dưới:

```js
const express = require('express')
const app = express()
const port = 3000

app.get('/', function (req, res) {
  res.send('Hello World')
})

app.listen(port, () => console.log(`Example app listening on port ${port}!`))
```

Đoạn mã trên dùng để tạo ra một máy chủ web lắng nghe với cổng (port) `3000`. Các request (yêu cầu) được gửi đến đường dẫn gốc (root URL) `/` sẽ được phản hồi lại nội dung `Hello World`.

Để khởi động máy chủ, sử dụng Terminal và nhập:

```console
node <tên file>.js
```

Nội dung `Example app listening on port 3000` sẽ được log trên Terminal khi khởi chạy thành công máy chủ.

Lúc này, mở trình duyệt và truy cập vào `localhost:3000`. Ta có thể thấy dòng chữ `Hello World` hiển thị tại đó.

Ta có thể chỉ định lại lệnh chạy máy chủ bằng `npm` bằng cách như sau:

- Mở file `package.json`

- Tìm đến khoá `"scripts"` và thêm vào như sau:

```json
  ...
  "scripts": {
    ...
    "start": "node <tên file>.js"
  }
  ...
```

- Sử dụng `Ctrl` + `C` để tắt máy chủ (nếu đang bật)

- Từ giờ, ta có thể khởi động máy chủ Express.js bằng lệnh `npm start`


## Cài đặt Nodemon

Cứ mỗi thay đổi, máy chủ cần phải khởi động lại để cập nhật. Nodemon giúp tự động khởi động lại máy chủ và ta không cần khởi động lại thủ công.

Sử dụng lệnh sau để cài đặt Nodemon:

```console
npm install -g nodemon
```

Sau khi quá trình cài đặt hoàn tất, thay đổi khoá `"scripts"` trong file `package.json` như sau:

```json
  ...
  "scripts": {
    ...
    "start": "nodemon <tên file>.js"
  }
  ...
```

Như vậy,các thay đổi về nội dung trong máy chủ không cần phải khởi động lại một cách thủ công.
