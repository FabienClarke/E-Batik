<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 1500 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[Many](https://www.many.co.uk)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[OP.GG](https://op.gg)**
- **[WebReinvent](https://webreinvent.com/?utm_source=laravel&utm_medium=github&utm_campaign=patreon-sponsors)**
- **[Lendio](https://lendio.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

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









