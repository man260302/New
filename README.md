# Lưu ý

## Phân tích:

`2023-07-19`: Năm - Tháng - Ngày

`---------`: Giờ : Phút : Giây

`+07:00[Asia/Bangkok]`: Múi giờ


## Quyền truy cập: Admin

### login

API login

Công dụng: đăng nhập

Url:http://localhost:3000/api/admin/login

Method: Post

Request:

```raw + json

{

   "username": "admin",

   "password": "12345"
   

}

Response:

{

    "success": true,
    
    "message": "Authentication successful",
    
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpYXQiOjE2ODk3NDgwMjQsImV4cCI6MTY4OTc1MTYyNH0.UZkT4s3drmJKhEIps2s6LVEBdO7TwkQ_iW0jmgpNL5s"
    
}
