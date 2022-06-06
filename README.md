

## Endpoint 

- Admin Login 
- Admin Refresh  
- Admin Logout 
- Admin Dashboard 
- Admin Categories 
- Admin Add Categories 
- Admin Get Data Categories 
- Admin Update Categories Data 
- Admin Delete Data Categories 
- Admin Products 
- Admin Add Products 
- Admin Get Add Products 
- Admin Update Products 
- Admin Delete Products 
- Admin Invoices 
- Admin Customers 
- Admin Get Sliders
- Admin Add Sliders 
- Admin Delete Sliders 
- Admin Get Users

## Users 

- Admin Get Users 
- Admin Update Users 
- Admin Add Users 
- Admin Delete Users 


## Website RestFull API 

- Get Categories 
- Show Categories 
- Show Categories Products 
- Get Sliders 
- Get Provinsi 
- Get Cities 
- Check Ongkir 
- Carts 
- Add Carts 
- Total Carts 


# API Documentation 

### Admin Login 
- Method     : POST 
Request:
  - Method : GET
  - Endpoint : http://localhost:8000/api/admin/login
  - Header : 
  
          Accept: application/json
          Content-Type: application/json
          Authorization: JWT
  
  - Body   : 
  
          email: admin@gmail.com
          password: ******
  
  - Respone:

          {
              "success": true,
              "user": {
                  "id": 1,
                  "name": "Administrator",
                  "email": "admin@gmail.com",
                  "email_verified_at": null,
                  "created_at": null,
                  "updated_at": null
              },
              "token":     "token"
          }
        
   - Code : 
   
   
         200 


## ADMIN
Admin Login
```json
"Method" : "POST"
"URL" : "http://localhost:8000/api/admin/login"
"Body" : 
"Email" : "required"
"Password" : "required"
"Headers" :
{"Accept" : "application/json"
"Content-Type" : "application/json"}
"Response" :
{
    "success": true,
    "user": {
        "id": 1,
        "name": "Administrator",
        "email": "admin@gmail.com",
        "email_verified_at": null,
        "created_at": null,
        "updated_at": null
    },
    "token":   "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJodHRwOlwvXC9sb2NhbGhvc3Q6ODAwMFwvYXBpXC9hZG1pblwvbG9naW4iLCJpYXQiOjE2NTQyNDI4MTQsImV4cCI6MTY1NDI0NjQxNCwibmJmIjoxNjU0MjQyODE0LCJqdGkiOiI5RjJrU05hckprbGNVUVhRIiwic3ViIjoxLCJwcnYiOiIyM2JkNWM4OTQ5ZjYwMGFkYjM5ZTcwMWM0MDA4NzJkYjdhNTk3NmY3In0.v5Hix5-GQX5e-_T-mO2EPGu5AUw9s60nCW7-0m-89KY"
}

"Code" : "200"
```
Admin Refresh
```json
"Method" : "GET"
"URL" : "http://localhost:8000/api/admin/refresh"
"Body" : 
"Headers" : 
{"Accept" : "application/json"
"Content-Type" : "application/json"}
"Response" :
{
    "success": true,
    "user": {
        "id": 1,
        "name": "Administrator",
        "email": "admin@gmail.com",
        "email_verified_at": null,
        "created_at": null,
        "updated_at": null
    },
    "token":   "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJodHRwOlwvXC9sb2NhbGhvc3Q6ODAwMFwvYXBpXC9hZG1pblwvbG9naW4iLCJpYXQiOjE2NTQyNDI4MTQsImV4cCI6MTY1NDI0NjQxNCwibmJmIjoxNjU0MjQyODE0LCJqdGkiOiI5RjJrU05hckprbGNVUVhRIiwic3ViIjoxLCJwcnYiOiIyM2JkNWM4OTQ5ZjYwMGFkYjM5ZTcwMWM0MDA4NzJkYjdhNTk3NmY3In0.v5Hix5-GQX5e-_T-mO2EPGu5AUw9s60nCW7-0m-89KY"
}
"Code" : "200"
```
Admin Invoices
```json
"Method" : "GET"
"URL" : "http://localhost:8000/api/admin/Invoices"
"Body" :
{"Email" : "required"
"Password" : "required"}
"Headers" :
{"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"}
"Response" :
{
    "success": true,
    "message": "List Data Invoices",
    "data": {
        "current_page": 1,
        "data": [
            {
                "id": 6,
                "invoice": "INV-F6N9J610TX",
                "customer_id": 4,
                "courier": "tiki",
                "courier_service": "REG",
                "courier_cost": 11000,
                "weight": 500,
                "name": "Rizqi Maulana",
                "phone": "85785852224",
                "city_id": 348,
                "province_id": 10,
                "address": "Pekalongan",
                "status": "pending",
                "grand_total": 495030,
                "snap_token": "424eeb7e-5280-4122-8447-d53048b1c3db",
                "created_at": "2021-08-03T06:55:03.000000Z",
                "updated_at": "2021-08-03T06:55:03.000000Z",
                "customer": {
                    "id": 4,
                    "name": "Rizqi Maulana",
                    "email": "rizqi@gmail.com",
                    "email_verified_at": null,
                    "created_at": "Kamis, 29 Juli 2021",
                    "updated_at": "2021-07-29T03:58:25.000000Z"
                }
            },
            {
                "id": 5,
                "invoice": "INV-38KTH9912E",
                "customer_id": 4,
                "courier": "jne",
                "courier_service": "REG",
                "courier_cost": 11000,
                "weight": 500,
                "name": "Rizqi Maulana",
                "phone": "85785852224",
                "city_id": 349,
                "province_id": 10,
                "address": "Pekalongan",
                "status": "pending",
                "grand_total": 865050,
                "snap_token": "e49cb35c-c567-4a04-a1a5-b9ae977a7ebc",
                "created_at": "2021-08-03T06:54:11.000000Z",
                "updated_at": "2021-08-03T06:54:11.000000Z",
                "customer": {
                    "id": 4,
                    "name": "Rizqi Maulana",
                    "email": "rizqi@gmail.com",
                    "email_verified_at": null,
                    "created_at": "Kamis, 29 Juli 2021",
                    "updated_at": "2021-07-29T03:58:25.000000Z"
                }
            },
            {
                "id": 4,
                "invoice": "INV-E30D94DRK9",
                "customer_id": 4,
                "courier": "jne",
                "courier_service": "OKE",
                "courier_cost": 10000,
                "weight": 500,
                "name": "Rizqi Maulana",
                "phone": "85785852224",
                "city_id": 349,
                "province_id": 10,
                "address": "Pekalongan",
                "status": "pending",
                "grand_total": 128680,
                "snap_token": "2228cb62-3c43-429e-98ea-6d7fc41189e2",
                "created_at": "2021-08-03T06:52:31.000000Z",
                "updated_at": "2021-08-03T06:52:36.000000Z",
                "customer": {
                    "id": 4,
                    "name": "Rizqi Maulana",
                    "email": "rizqi@gmail.com",
                    "email_verified_at": null,
                    "created_at": "Kamis, 29 Juli 2021",
                    "updated_at": "2021-07-29T03:58:25.000000Z"
                }
            },
            {
                "id": 3,
                "invoice": "INV-VSKP9K0RV3",
                "customer_id": 4,
                "courier": "jne",
                "courier_service": "OKE",
                "courier_cost": 10000,
                "weight": 500,
                "name": "Rizqi Maulana",
                "phone": "85785852224",
                "city_id": 349,
                "province_id": 10,
                "address": "Pekalongan",
                "status": "pending",
                "grand_total": 494030,
                "snap_token": "d0c395e5-3ab3-4de5-ad3c-0c7b56f0f423",
                "created_at": "2021-08-03T06:50:45.000000Z",
                "updated_at": "2021-08-03T06:50:50.000000Z",
                "customer": {
                    "id": 4,
                    "name": "Rizqi Maulana",
                    "email": "rizqi@gmail.com",
                    "email_verified_at": null,
                    "created_at": "Kamis, 29 Juli 2021",
                    "updated_at": "2021-07-29T03:58:25.000000Z"
                }
            },
            {
                "id": 2,
                "invoice": "INV-67UC3G8766",
                "customer_id": 4,
                "courier": "jne",
                "courier_service": "OKE",
                "courier_cost": 10000,
                "weight": 200,
                "name": "Rizqi Maulana",
                "phone": "85785852224",
                "city_id": 348,
                "province_id": 10,
                "address": "Pekalongan",
                "status": "pending",
                "grand_total": 58020,
                "snap_token": "050ac6b7-38f6-4ac7-809c-2829e5b2a938",
                "created_at": "2021-08-03T06:48:46.000000Z",
                "updated_at": "2021-08-03T06:48:46.000000Z",
                "customer": {
                    "id": 4,
                    "name": "Rizqi Maulana",
                    "email": "rizqi@gmail.com",
                    "email_verified_at": null,
                    "created_at": "Kamis, 29 Juli 2021",
                    "updated_at": "2021-07-29T03:58:25.000000Z"
                }
            }
        ],
        "first_page_url": "http://localhost:8000/api/admin/invoices?page=1",
        "from": 1,
        "last_page": 2,
        "last_page_url": "http://localhost:8000/api/admin/invoices?page=2",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "http://localhost:8000/api/admin/invoices?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": "http://localhost:8000/api/admin/invoices?page=2",
                "label": "2",
                "active": false
            },
            {
                "url": "http://localhost:8000/api/admin/invoices?page=2",
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "next_page_url": "http://localhost:8000/api/admin/invoices?page=2",
        "path": "http://localhost:8000/api/admin/invoices",
        "per_page": 5,
        "prev_page_url": null,
        "to": 5,
        "total": 6
    }
}
"Code" : "200"
```

Admin Customers
```json
"Method" : "GET"
"URL" : "http://localhost:8000/api/admin/Customers"
"Body" 
"Email" : "required"
"Password" : "required"
"Headers" :
{"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"}
"Response" :
{
    "success": true,
    "message": "List Data Customer",
    "data": {
        "current_page": 1,
        "data": [
            {
                "id": 5,
                "name": "alex",
                "email": "alex18@gmail.com",
                "email_verified_at": null,
                "created_at": "Minggu, 29 Mei 2022",
                "updated_at": "2022-05-29T10:09:56.000000Z"
            },
            {
                "id": 4,
                "name": "Rizqi Maulana",
                "email": "rizqi@gmail.com",
                "email_verified_at": null,
                "created_at": "Kamis, 29 Juli 2021",
                "updated_at": "2021-07-29T03:58:25.000000Z"
            },
            {
                "id": 2,
                "name": "Yudi Purwanto",
                "email": "yudi@gmail.com",
                "email_verified_at": null,
                "created_at": "Kamis, 29 Juli 2021",
                "updated_at": "2021-07-29T03:56:43.000000Z"
            },
            {
                "id": 1,
                "name": "Kurnia Andi Nugroho",
                "email": "kurnia@gmail.com",
                "email_verified_at": null,
                "created_at": "Kamis, 15 Juli 2021",
                "updated_at": "2021-07-15T03:34:32.000000Z"
            }
        ],
        "first_page_url": "http://localhost:8000/api/admin/customers?page=1",
        "from": 1,
        "last_page": 1,
        "last_page_url": "http://localhost:8000/api/admin/customers?page=1",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "http://localhost:8000/api/admin/customers?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": null,
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "next_page_url": null,
        "path": "http://localhost:8000/api/admin/customers",
        "per_page": 5,
        "prev_page_url": null,
        "to": 4,
        "total": 4
    }
}
"Code" : "200"
```
Admin Sliders
```json
"Method" : "GET"
"URL" : "http://localhost:8000/api/admin/Sliders"
"Body" :
"Headers" : 
{"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"}
"Response" : 
{
    "success": true,
    "message": "List Data Sliders",
    "data": {
        "current_page": 1,
        "data": [
            {
                "id": 5,
                "image": "http://localhost:8000/storage/sliders/zaxsS4mEijjBElfifyVkTvVLM99UizMCZc2ZmFrm.jpg",
                "link": "google.com",
                "created_at": "2022-05-22T23:23:20.000000Z",
                "updated_at": "2022-05-22T23:23:20.000000Z"
            },
            {
                "id": 4,
                "image": "http://localhost:8000/storage/sliders/qUYu2FOZPsR3beNrSwvRw6m29QMZLijUuZvyjybD.png",
                "link": "#",
                "created_at": "2021-07-30T12:35:57.000000Z",
                "updated_at": "2021-07-30T12:35:57.000000Z"
            },
            {
                "id": 3,
                "image": "http://localhost:8000/storage/sliders/2wxXb5XyqGJqy9YF0WsZ22zx5fWGHv48iLAZVS3o.png",
                "link": "#",
                "created_at": "2021-07-30T12:35:50.000000Z",
                "updated_at": "2021-07-30T12:35:50.000000Z"
            }
        ],
        "first_page_url": "http://localhost:8000/api/admin/sliders?page=1",
        "from": 1,
        "last_page": 1,
        "last_page_url": "http://localhost:8000/api/admin/sliders?page=1",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "http://localhost:8000/api/admin/sliders?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": null,
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "next_page_url": null,
        "path": "http://localhost:8000/api/admin/sliders",
        "per_page": 5,
        "prev_page_url": null,
        "to": 3,
        "total": 3
    }
}
"Code" : "200"
```
Admin sliders add
```json
"Method" : "POST"
"URL" : "http://localhost:8000/api/admin/Customers"
"Body" :
"Image" : "Nama.JPG"
"Link" : "url"
"Headers" :
{"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"}
"Response" :
{
    "success": true,
    "message": "Data Slider Berhasil Disimpan!",
    "data": {
        "image": "http://localhost:8000/storage/sliders/TCZQJBmAbDfpGHp6kx3sxTSJxRb4Ci9ppcKKYPIa.jpg",
        "link": "#",
        "updated_at": "2022-06-04T08:55:20.000000Z",
        "created_at": "2022-06-04T08:55:20.000000Z",
        "id": 7
    }
}
"Code" : "200"
```
Admin Sliders Delete
```json
"Method" : "DELETE"
"URL" : "http://localhost:8000/api/admin/sliders/7"
"Body" :
{"Image" : "Nama.JPG"
"Link" : "url"}
"Headers" :
{"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"}
"Response" :
{
    "success": true,
    "message": "Data Slider Berhasil Dihapus!",
    "data": null
}
"Code" : "200"
```
Admin Categories Post
```json
"Method" : "Post"
"URL" : "http://localhost:8000/api/admin/categories"
"Body" :
{"Image" : "Nama.jpg"
"Name" : "Batik Parang"}
"Headers" :
{"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"}
"Response" :
{
    "success": true,
    "message": "Data Category Berhasil Disimpan!",
    "data": {
        "image": "http://localhost:8000/storage/categories/gJNFQ9PnYVm5YERgk5VuTZkJyUcic7rGsTW0TTTA.jpg",
        "name": "Batik Parang",
        "slug": "batik-parang",
        "updated_at": "2022-06-04T09:06:14.000000Z",
        "created_at": "2022-06-04T09:06:14.000000Z",
        "id": 11
    }
}
 
"Code" : "200"
```
Admin Get User
```json
"Method" : "GET",
"URL" : "http://localhost:8000/api/admin/user",
"Body" :
"Headers" :
{"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"}
"Response" :
{
    "success": true,
    "user": {
        "id": 1,
        "name": "Administrator",
        "email": "admin@gmail.com",
        "email_verified_at": null,
        "created_at": null,
        "updated_at": null
    }
}
"Code" : "200"
```









