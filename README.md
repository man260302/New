# Lưu ý

## Phân tích:

`2023-07-19`: Năm - Tháng - Ngày

`---------`: Giờ : Phút : Giây

`+07:00[Asia/Bangkok]`: Múi giờ


## Quyền truy cập: Admin

### login

API: login

Công dụng: đăng nhập

Url:http://localhost:3000/api/admin/login

Method: Post

Request:

```json

{
   "username": "admin",
   "password": "12345"
}

```

Response:

```json

{
    "success": true,
    "message": "Authentication successful",
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpYXQiOjE2ODk3NDgwMjQsImV4cCI6MTY4OTc1MTYyNH0.UZkT4s3drmJKhEIps2s6LVEBdO7TwkQ_iW0jmgpNL5s"
}

```

### Token

API: token

Công dụng: lấy token đăng nhập

Url:http://localhost:3000/api/admin/token

Method: Get

Request:

| Key           | Value         |
|---------------|---------------|
|x-access-token |eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpYXQiOjE2ODk3NDgwMjQsImV4cCI6MTY4OTc1MTYyNH0.UZkT4s3drmJKhEIps2s6LVEBdO7TwkQ_iW0jmgpNL5s |

Response:

```json

{
    "success": true,
    "message": "Token is valid",
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpYXQiOjE2ODk3NDgwMjQsImV4cCI6MTY4OTc1MTYyNH0.UZkT4s3drmJKhEIps2s6LVEBdO7TwkQ_iW0jmgpNL5s"
}

```

### Categories

API: categories

Công dụng: chứa các ID của product

Url:http://localhost:3000/api/admin/categories

Method: Get

Request:

| Key           | Value         |
|---------------|---------------|
|x-access-token |eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpYXQiOjE2ODk3NDgwMjQsImV4cCI6MTY4OTc1MTYyNH0.UZkT4s3drmJKhEIps2s6LVEBdO7TwkQ_iW0jmgpNL5s |

Response:

```json

[
    {
        "_id": "6288b174708fabf8ab29ca0d",
        "name": "iPhone"
    },
    {
        "_id": "6288b180708fabf8ab29ca10",
        "name": "Macbook"
    },
    {
        "_id": "647961dacabbcb41554ca355",
        "name": "iPad"
    },
    {
        "_id": "647965aeb04462d60e8e41b3",
        "name": "iPone2"
    },
    {
        "_id": "64a4e4d8014f83f098c27ccc",
        "name": "Kemduong"
    },
    {
        "_id": "64a4f201014f83f098c27d0d",
        "name": "iPhone"
    }
]

```
### Categories

API: post name categories

Công dụng: đăng các categories lên

Url:http://localhost:3000/api/admin/categories

Method: Post

Request:
+ Headers:

| Key           | Value         |
|---------------|---------------|
|x-access-token |eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpYXQiOjE2ODk3NDgwMjQsImV4cCI6MTY4OTc1MTYyNH0.UZkT4s3drmJKhEIps2s6LVEBdO7TwkQ_iW0jmgpNL5s |

+ Body
  
```json
{
    "name": "iPad"
}
```

Response:

```json
{
    "_id": "64b7fdd7dd1100adf12fb6f8",
    "name": "iPad"
}
```

