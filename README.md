

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
"Headers" 
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
"Headers"  
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
"Headers" 
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
"Headers" 
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
"Headers"  
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
"Headers" 
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
"Headers" 
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
"Headers" 
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
"Headers" 
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
## WEBSITE
Categories
```
- Name: Catagories
- Method:Get
- URL: http://localhost:8000/api/web/categories
- Body:
- Headers:
    Accept: application/json
    Content-Type: application/json
    
 - Response: {
    "success": true,
    "message": "List Data Categories",
    "data": [
        {
            "id": 10,
            "name": "batik contoh 5",
            "slug": "batik-contoh-5",
            "image": "http://localhost:8000/storage/categories/nbD6gkryhyhT9RTfoKHFnAGPEUJgcsVPjieYQb2A.jpg",
            "created_at": "2022-05-23T07:13:00.000000Z",
            "updated_at": "2022-05-23T07:13:00.000000Z"
        },
        {
            "id": 9,
            "name": "Batik Lamongan",
            "slug": "batik-lamongan",
            "image": "http://localhost:8000/storage/categories/hmvTMkgTSaykHTBSbeqW3s5CRwOnT12LSnQtHj3A.jpg",
            "created_at": "2022-05-23T06:17:05.000000Z",
            "updated_at": "2022-05-23T06:17:05.000000Z"
        },
        {
            "id": 6,
            "name": "batik Megamendung",
            "slug": "batik-megamendung",
            "image": "http://localhost:8000/storage/categories/0EiWmkdUml3e6jN7ghdUMdkk1w6aEPAzJoNwvhTI.jpg",
            "created_at": "2022-05-22T21:18:10.000000Z",
            "updated_at": "2022-05-22T21:18:10.000000Z"
        }
    ]
}
```

## CUSTOMER
Customer Register
```json
"Method" : "POST"
"URL" : "http://localhost:8000/api/customer/register"
"Body" :
"Name" : "Aldi"
"Email" : "aldi@gmail.com"
"Password" : "password"
"Password_confirmation" : "password"
"Headers"
"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"
"Response"
{
    "success": true,
    "message": "Register Customer Berhasil",
    "data": {
        "name": "rainer",
        "email": "rainer@gmail.com",
        "updated_at": "2022-06-04T12:39:45.000000Z",
        "created_at": "Sabtu, 04 Juni 2022",
        "id": 6
    }
}
 
"Code" : "200"
```
Customer Login
```json
"Method" : "POST"
"URL" : "http://localhost:8000/api/customer/login"
"Body"
"Email" : "Email@gmail.com"
"Password" : "passwod"
"Headers"
"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"
"Response"
{
    "success": true,
    "user": {
        "id": 6,
        "name": "rainer",
        "email": "rainer@gmail.com",
        "email_verified_at": null,
        "created_at": "Sabtu, 04 Juni 2022",
        "updated_at": "2022-06-04T12:39:45.000000Z"
    },
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJodHRwOi8vbG9jYWxob3N0OjgwMDAvYXBpL2N1c3RvbWVyL2xvZ2luIiwiaWF0IjoxNjU0MzQ2NTA2LCJleHAiOjE2NTQzNTAxMDYsIm5iZiI6MTY1NDM0NjUwNiwianRpIjoidENrcXg1ejVobUVHMjdVVyIsInN1YiI6IjYiLCJwcnYiOiIxZDBhMDIwYWNmNWM0YjZjNDk3OTg5ZGYxYWJmMGZiZDRlOGM4ZDYzIn0.74mw9SwF-bYMx8YV1wX6J4JZB2dQsEMl-m-kZCayMHU"
}
 
"Code" : "200"
```
GET Customer After Login
```json
"Method" : "GET"
"URL" : "http://localhost:8000/api/customer/user"
"Body"
"Headers"
"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"
"Response"
{
    "success": true,
    "user": {
        "id": 6,
        "name": "rainer",
        "email": "rainer@gmail.com",
        "email_verified_at": null,
        "created_at": "Sabtu, 04 Juni 2022",
        "updated_at": "2022-06-04T12:39:45.000000Z"
    }
}
 
"Code" : "200"
```
Refresh Customer
```json
"Method" : "GET"
"URL" : "http://localhost:8000/api/customer/refresh"
"Body"
"Headers"
"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"
"Response"
{
    "success": true,
    "user": {
        "id": 6,
        "name": "rainer",
        "email": "rainer@gmail.com",
        "email_verified_at": null,
        "created_at": "Sabtu, 04 Juni 2022",
        "updated_at": "2022-06-04T12:39:45.000000Z"
    },
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJodHRwOi8vbG9jYWxob3N0OjgwMDAvYXBpL2N1c3RvbWVyL3JlZnJlc2giLCJpYXQiOjE2NTQzNDY1MDYsImV4cCI6MTY1NDM1MDIwMywibmJmIjoxNjU0MzQ2NjAzLCJqdGkiOiJsc0NtZGF5Mk1GeklNRVcwIiwic3ViIjoiNiIsInBydiI6IjFkMGEwMjBhY2Y1YzRiNmM0OTc5ODlkZjFhYmYwZmJkNGU4YzhkNjMifQ.6zLgcJri4GzpGbK0Ie6bg4QuhtVdZQQj8xeJoDVX7EU"
}
 
"Code" : "200"
```
Logout
```json
"Method" : "POST"
"URL" : "http://localhost:8000/api/customer/logout"
"Body"
"Headers"
"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"
"Response"
{
    "success": true
}
 
"Code" : "200"
```
Dashboard
```json
"Method" : "GET"
"URL" : "http://localhost:8000/api/customer/dashboard"
"Body" 
"Headers"
"Accept" : "application/json"
"Content-Type" : "application/json"
"Response"
{
    "success": true,
    "message": "Statistik Data",
    "data": {
        "count": {
            "pending": 0,
            "success": 0,
            "expired": 0,
            "failed": 0
        }
    }
}
 
"Code" : "200"
```
InVoice
```json
"Method" : "GET"
"URL" : "http://localhost:8000/api/customer/invoices"
"Body"
"Headers"
"Accept" : "application/json"
"Content-Type" : "application/json"
"Authorization" : "Bearer Token"
"Response"
{
    "success": true,
    "message": "List Data Invoices : rainer",
    "data": {
        "current_page": 1,
        "data": [],
        "first_page_url": "http://localhost:8000/api/customer/invoices?page=1",
        "from": null,
        "last_page": 1,
        "last_page_url": "http://localhost:8000/api/customer/invoices?page=1",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "http://localhost:8000/api/customer/invoices?page=1",
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
        "path": "http://localhost:8000/api/customer/invoices",
        "per_page": 5,
        "prev_page_url": null,
        "to": null,
        "total": 0
    }
}
"Code" : "200"
```





## WEBSITE
Categories
```
- Method:Get
- URL: http://localhost:8000/api/web/categories
- Body:
- Headers:
    Accept: application/json
    Content-Type: application/json
    
 - Response: {
    "success": true,
    "message": "List Data Categories",
    "data": [
        {
            "id": 10,
            "name": "batik contoh 5",
            "slug": "batik-contoh-5",
            "image": "http://localhost:8000/storage/categories/nbD6gkryhyhT9RTfoKHFnAGPEUJgcsVPjieYQb2A.jpg",
            "created_at": "2022-05-23T07:13:00.000000Z",
            "updated_at": "2022-05-23T07:13:00.000000Z"
        },
        {
            "id": 9,
            "name": "Batik Lamongan",
            "slug": "batik-lamongan",
            "image": "http://localhost:8000/storage/categories/hmvTMkgTSaykHTBSbeqW3s5CRwOnT12LSnQtHj3A.jpg",
            "created_at": "2022-05-23T06:17:05.000000Z",
            "updated_at": "2022-05-23T06:17:05.000000Z"
        },
        {
            "id": 6,
            "name": "batik Megamendung",
            "slug": "batik-megamendung",
            "image": "http://localhost:8000/storage/categories/0EiWmkdUml3e6jN7ghdUMdkk1w6aEPAzJoNwvhTI.jpg",
            "created_at": "2022-05-22T21:18:10.000000Z",
            "updated_at": "2022-05-22T21:18:10.000000Z"
        }
    ]
}
```

## Users
Admin Get Users
```
- Method:Get
- URL:  http://localhost:8000/api/admin/users
- Body:
- Headers:
    Accept: application/json
    Content-Type: application/json
    Authorization: Bearer "Token"

Response: {
    "success": true,
    "message": "List Data Users",
    "data": {
        "current_page": 1,
        "data": [
            {
                "id": 2,
                "name": "Mulyadi Arman",
                "email": "mulyadiarman18@gmail.com",
                "email_verified_at": null,
                "created_at": "2022-06-06T01:46:14.000000Z",
                "updated_at": "2022-06-06T01:46:14.000000Z"
            },
            {
                "id": 1,
                "name": "Administrator",
                "email": "admin@gmail.com",
                "email_verified_at": null,
                "created_at": null,
                "updated_at": null
            }
        ],
        "first_page_url": "http://localhost:8000/api/admin/users?page=1",
        "from": 1,
        "last_page": 1,
        "last_page_url": "http://localhost:8000/api/admin/users?page=1",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "http://localhost:8000/api/admin/users?page=1",
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
        "path": "http://localhost:8000/api/admin/users",
        "per_page": 5,
        "prev_page_url": null,
        "to": 2,
        "total": 2
    }
}
```

Admin Update Users
```
- Method: Post
- URL:  http://localhost:8000/api/admin/users/2
- Body:
    email: mulyadiarman18@gmail.com
    password: password
    password_confirmation: password
    _method: PATCH
- Headers:
    Content-Type: application/json
    Accept: application/json
    Authorization: Bearer "Token"
 
 - Response: {
    "success": true,
    "message": "Data User Berhasil Diupdate!",
    "data": {
        "id": 2,
        "name": "Mulyadi Arman123",
        "email": "mulyadiarman18@gmail.com",
        "email_verified_at": null,
        "created_at": "2022-06-06T01:46:14.000000Z",
        "updated_at": "2022-06-06T02:44:55.000000Z"
    }
}
```

Admin Post Users
```
- Method: Post
- URL:  http://localhost:8000/api/admin/users
- Body:
    name: SatrioPutra
    email: satriopewee@gmail.com
    password: password
    password_confirmation: password
- Headers:
    Accept: application/json
    Content-Type: application/json
    Authorization: Bearer "Token"
    
- Response:{
    "success": true,
    "message": "Data User Berhasil Disimpan!",
    "data": {
        "name": "SatrioPutra",
        "email": "satriopewee@gmail.com",
        "updated_at": "2022-06-06T02:58:36.000000Z",
        "created_at": "2022-06-06T02:58:36.000000Z",
        "id": 4
    }
}
```

Delete Users
```
- Method: Delete
- URL:  http://localhost:8000/api/admin/users/2
- Body: 
    name: Mulyadi Arman123
    email: mulyadiarman18@gmail.com
    password: password
    password_confirmation: password
- Headers:
    Content-Type: application/json
    Accept: application/json
    Authorization: Bearer "Token"
- Response: {
    "success": true,
    "message": "Data User Berhasil Dihapus!",
    "data": null
}
```

## WEBSITE 

List Data Categories 
Request:
  - Method : GET
  - Endpoint : http://localhost:8000/api/web/categories
  - Header : 
  
          Accept: application/json
          Content-Type: application/json
          
  
  - Body   : 
  
          
  
  - Respone: 
  
                {
                    "success": true,
                    "message": "List Data Categories",
                    "data": [
                        {
                            "id": 2,
                            "name": "batik parang rusak",
                            "slug": "batik-parang-rusak",
                            "image": "http://localhost:8000/storage/categories/G3ktsny0ntUjvzeHFyOQfDiAghFvb42gSn5oQ074.jpg",
                            "created_at": "2022-05-29T20:31:36.000000Z",
                            "updated_at": "2022-06-03T07:34:19.000000Z"
                        },
                        {
                            "id": 1,
                            "name": "barang 2",
                            "slug": "barang-2",
                            "image": "http://localhost:8000/storage/categories/qhkvkK1spEeEQDjUoWxXjFhtrFJAdI7vLWgiQ5fb.jpg",
                            "created_at": "2022-05-29T17:03:39.000000Z",
                            "updated_at": "2022-05-29T21:05:54.000000Z"
                        }
                    ]
                }
 


Show Data Categories 
Request:
  - Method : GET
  - Endpoint : http://localhost:8000/api/web/categories/batik-nugroho
  - Header : 
  
          Accept: application/json
          Content-Type: application/json
          
  
  - Body   : 
  
          
  
  - Respone: 

                {
                    "success": true,
                    "message": "Data Product By Category : batik parang rusak",
                    "data": {
                        "id": 2,
                        "name": "batik parang rusak",
                        "slug": "batik-parang-rusak",
                        "image": "http://localhost:8000/storage/categories/G3ktsny0ntUjvzeHFyOQfDiAghFvb42gSn5oQ074.jpg",
                        "created_at": "2022-05-29T20:31:36.000000Z",
                        "updated_at": "2022-06-03T07:34:19.000000Z",
                        "products": []
                    }
                }


Show Detail Data Products
Request:
  - Method : GET
  - Endpoint : http://localhost:8000/api/web/products/bating-lengan-panjan-nugroho
  - Header : 
  
          Accept: application/json
          Content-Type: application/json
          
  
  - Body   : 
  
          
  
  - Respone: 



                    {
                        "success": true,
                        "message": "Detail Data Product!",
                        "data": {
                            "id": 1,
                            "image": "http://localhost:8000/storage/products/G63skJFShsMIzwicrjenzaIjoNCFHBCKQ5Qw69di.jpg",
                            "title": "Bating lengan panjan nugroho",
                            "slug": "bating-lengan-panjan-nugroho",
                            "category_id": 1,
                            "user_id": 1,
                            "description": "baju ini adalah baju yang di desain untuk kondangan dan acara besar",
                            "weight": 450,
                            "price": 900000,
                            "stock": 50,
                            "discount": 10,
                            "created_at": "2022-05-29T17:07:56.000000Z",
                            "updated_at": "2022-05-29T17:07:56.000000Z",
                            "reviews_avg_rating": "5.0",
                            "reviews_count": 1,
                            "category": {
                                "id": 1,
                                "name": "barang 2",
                                "slug": "barang-2",
                                "image": "http://localhost:8000/storage/categories/qhkvkK1spEeEQDjUoWxXjFhtrFJAdI7vLWgiQ5fb.jpg",
                                "created_at": "2022-05-29T17:03:39.000000Z",
                                "updated_at": "2022-05-29T21:05:54.000000Z"
                            },
                            "reviews": [
                                {
                                    "id": 1,
                                    "product_id": 1,
                                    "order_id": 2,
                                    "customer_id": 2,
                                    "rating": 5,
                                    "review": "sangat bagus",
                                    "created_at": "2022-05-30T05:50:06.000000Z",
                                    "updated_at": "2022-05-30T05:50:06.000000Z",
                                    "customer": {
                                        "id": 2,
                                        "name": "mulyadi arman",
                                        "email": "mulyadiarman18@gmail.com",
                                        "email_verified_at": null,
                                        "created_at": "Minggu, 29 Mei 2022",
                                        "updated_at": "2022-05-29T22:11:42.000000Z"
                                    }
                                }
                            ]
                        }
                    }


Show Sliders 
Request:
  - Method : GET
  - Endpoint :  http://localhost:8000/api/web/sliders
  - Header : 
  
          Accept: application/json
          Content-Type: application/json
          
  
  - Body   : 
  
          
  
  - Respone: 

                {
                    "success": true,
                    "message": "List Data Sliders",
                    "data": []
                }


Show Ptovinces 
Request:
  - Method : GET
  - Endpoint :  http://localhost:8000/api/web/rajaongkir/provinces
  - Header : 
  
          Accept: application/json
          Content-Type: application/json
          
  
  - Body   : 
        
          
  
  - Respone: 

                {
                    "success": true,
                    "message": "List Data Provinces",
                    "data": [
                        {
                            "id": 1,
                            "province_id": 1,
                            "name": "Bali",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 2,
                            "province_id": 2,
                            "name": "Bangka Belitung",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 3,
                            "province_id": 3,
                            "name": "Banten",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 4,
                            "province_id": 4,
                            "name": "Bengkulu",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 5,
                            "province_id": 5,
                            "name": "DI Yogyakarta",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 6,
                            "province_id": 6,
                            "name": "DKI Jakarta",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 7,
                            "province_id": 7,
                            "name": "Gorontalo",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 8,
                            "province_id": 8,
                            "name": "Jambi",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 9,
                            "province_id": 9,
                            "name": "Jawa Barat",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 10,
                            "province_id": 10,
                            "name": "Jawa Tengah",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 11,
                            "province_id": 11,
                            "name": "Jawa Timur",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 12,
                            "province_id": 12,
                            "name": "Kalimantan Barat",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 13,
                            "province_id": 13,
                            "name": "Kalimantan Selatan",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 14,
                            "province_id": 14,
                            "name": "Kalimantan Tengah",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 15,
                            "province_id": 15,
                            "name": "Kalimantan Timur",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 16,
                            "province_id": 16,
                            "name": "Kalimantan Utara",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 17,
                            "province_id": 17,
                            "name": "Kepulauan Riau",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 18,
                            "province_id": 18,
                            "name": "Lampung",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 19,
                            "province_id": 19,
                            "name": "Maluku",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 20,
                            "province_id": 20,
                            "name": "Maluku Utara",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 21,
                            "province_id": 21,
                            "name": "Nanggroe Aceh Darussalam (NAD)",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 22,
                            "province_id": 22,
                            "name": "Nusa Tenggara Barat (NTB)",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 23,
                            "province_id": 23,
                            "name": "Nusa Tenggara Timur (NTT)",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 24,
                            "province_id": 24,
                            "name": "Papua",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 25,
                            "province_id": 25,
                            "name": "Papua Barat",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 26,
                            "province_id": 26,
                            "name": "Riau",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 27,
                            "province_id": 27,
                            "name": "Sulawesi Barat",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 28,
                            "province_id": 28,
                            "name": "Sulawesi Selatan",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 29,
                            "province_id": 29,
                            "name": "Sulawesi Tengah",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 30,
                            "province_id": 30,
                            "name": "Sulawesi Tenggara",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 31,
                            "province_id": 31,
                            "name": "Sulawesi Utara",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 32,
                            "province_id": 32,
                            "name": "Sumatera Barat",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 33,
                            "province_id": 33,
                            "name": "Sumatera Selatan",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        },
                        {
                            "id": 34,
                            "province_id": 34,
                            "name": "Sumatera Utara",
                            "created_at": "2022-05-29T17:36:01.000000Z",
                            "updated_at": "2022-05-29T17:36:01.000000Z"
                        }
                    ]
                }
                
   
Show City 
Request:
  - Method : GET
  - Endpoint :  http://localhost:8000/api/web/rajaongkir/cities
  - Header : 
  
          Accept: application/json
          Content-Type: application/json
          
  
  - Body   : 
        
        provinces_id: 1  
  
  - Respone: 


                {
                    "success": true,
                    "message": "List Data City By Province : Bali",
                    "data": [
                        {
                            "id": 17,
                            "province_id": 1,
                            "city_id": 17,
                            "name": "Badung - (Kabupaten)",
                            "created_at": "2022-05-29T17:37:07.000000Z",
                            "updated_at": "2022-05-29T17:37:07.000000Z"
                        },
                        {
                            "id": 32,
                            "province_id": 1,
                            "city_id": 32,
                            "name": "Bangli - (Kabupaten)",
                            "created_at": "2022-05-29T17:37:07.000000Z",
                            "updated_at": "2022-05-29T17:37:07.000000Z"
                        },
                        {
                            "id": 94,
                            "province_id": 1,
                            "city_id": 94,
                            "name": "Buleleng - (Kabupaten)",
                            "created_at": "2022-05-29T17:37:07.000000Z",
                            "updated_at": "2022-05-29T17:37:07.000000Z"
                        },
                        {
                            "id": 114,
                            "province_id": 1,
                            "city_id": 114,
                            "name": "Denpasar - (Kota)",
                            "created_at": "2022-05-29T17:37:07.000000Z",
                            "updated_at": "2022-05-29T17:37:07.000000Z"
                        },
                        {
                            "id": 128,
                            "province_id": 1,
                            "city_id": 128,
                            "name": "Gianyar - (Kabupaten)",
                            "created_at": "2022-05-29T17:37:07.000000Z",
                            "updated_at": "2022-05-29T17:37:07.000000Z"
                        },
                        {
                            "id": 161,
                            "province_id": 1,
                            "city_id": 161,
                            "name": "Jembrana - (Kabupaten)",
                            "created_at": "2022-05-29T17:37:07.000000Z",
                            "updated_at": "2022-05-29T17:37:07.000000Z"
                        },
                        {
                            "id": 170,
                            "province_id": 1,
                            "city_id": 170,
                            "name": "Karangasem - (Kabupaten)",
                            "created_at": "2022-05-29T17:37:07.000000Z",
                            "updated_at": "2022-05-29T17:37:07.000000Z"
                        },
                        {
                            "id": 197,
                            "province_id": 1,
                            "city_id": 197,
                            "name": "Klungkung - (Kabupaten)",
                            "created_at": "2022-05-29T17:37:07.000000Z",
                            "updated_at": "2022-05-29T17:37:07.000000Z"
                        },
                        {
                            "id": 447,
                            "province_id": 1,
                            "city_id": 447,
                            "name": "Tabanan - (Kabupaten)",
                            "created_at": "2022-05-29T17:37:08.000000Z",
                            "updated_at": "2022-05-29T17:37:08.000000Z"
                        }
                    ]
                }
                
                
                
               
Check Ongkir 
Request:
  - Method : POST
  - Endpoint :  http://localhost:8000/api/web/rajaongkir/checkOngkir
  - Header : 
  
          Accept: application/json
          Content-Type: application/json
          
  
  - Body   : 
        
          destination : 144
          weight : 1000
          courier : jne
  
  - Respone: 
  
  
                      {
                        "success": true,
                        "message": "List Data Biaya Ongkos Kirim : jne",
                        "data": [
                            {
                                "service": "OKE",
                                "description": "Ongkos Kirim Ekonomis",
                                "cost": [
                                    {
                                        "value": 44000,
                                        "etd": "5-7",
                                        "note": ""
                                    }
                                ]
                            },
                            {
                                "service": "REG",
                                "description": "Layanan Reguler",
                                "cost": [
                                    {
                                        "value": 48000,
                                        "etd": "3-5",
                                        "note": ""
                                    }
                                ]
                            }
                        ]
                    }
                    
                    
                  
                   


carts
Request:
  - Method : GET
  - Endpoint :   http://localhost:8000/api/web/carts
  - Header : 
  
          Accept: application/json
          Content-Type: application/json
          Authorization: Bearer token
  
  - Body   : 
        
  
  - Respone: 


                    {
                        "success": true,
                        "message": "List Data Carts : alex",
                        "data": [
                            {
                                "id": 1,
                                "product_id": 1,
                                "customer_id": 1,
                                "qty": 1,
                                "price": 100000,
                                "weight": 100,
                                "created_at": "2022-05-29T19:02:44.000000Z",
                                "updated_at": "2022-05-29T19:02:44.000000Z",
                                "product": {
                                    "id": 1,
                                    "image": "http://localhost:8000/storage/products/G63skJFShsMIzwicrjenzaIjoNCFHBCKQ5Qw69di.jpg",
                                    "title": "Bating lengan panjan nugroho",
                                    "slug": "bating-lengan-panjan-nugroho",
                                    "category_id": 1,
                                    "user_id": 1,
                                    "description": "baju ini adalah baju yang di desain untuk kondangan dan acara besar",
                                    "weight": 450,
                                    "price": 900000,
                                    "stock": 50,
                                    "discount": 10,
                                    "created_at": "2022-05-29T17:07:56.000000Z",
                                    "updated_at": "2022-05-29T17:07:56.000000Z"
                                }
                            }
                        ]
                    }
                    

add carts 
Request:
  - Method : POST
  - Endpoint :   http://localhost:8000/api/web/carts
  - Header : 
  
          Accept: application/json
          Content-Type: application/json
          Authorization: Bearer token
  
  - Body   : 

          product_id: 1
          qty: 1
          price: 100000
          weight: 100
        
  
  - Respone:


                {
                    "success": true,
                    "message": "Success Add To Cart",
                    "data": {
                        "id": 1,
                        "product_id": 1,
                        "customer_id": 1,
                        "qty": 2,
                        "price": 200000,
                        "weight": 200,
                        "created_at": "2022-05-29T19:02:44.000000Z",
                        "updated_at": "2022-06-06T03:07:00.000000Z"
                    }
                }
                
                
                
                
                
Total carts 
Request:
  - Method : GET
  - Endpoint :    http://localhost:8000/api/web/carts/total_price
  - Header : 
  
          Accept: application/json
          Content-Type: application/json
          Authorization: Bearer token
  
  - Body   : 

          product_id: 1
          qty: 1
          price: 100000
          weight: 100
        
  
  - Respone: 
 
            {
                "success": true,
                "message": "Total Cart Price",
                "data": "200000"
            }
