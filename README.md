### DOKUMENTASI API

### 1. Tambah Data User Baru (Create)
Menambahkan data user baru. ID akan *digenerate* secara otomatis dalam bentuk UUID.

* URL: /api/users
* Method: POST
* Request Body:
    json
    {
        "name": "Hitam Legam",
        "age": 25
    }
    
* Success Response (201 Created):
```json
    {
        "status": "success",
        "data": {
            "id": "24f2da67-4c21-4c8b-b952-b8aa93d2eb03",
            "name": "Hitam Legam",
            "age": 25
        }
    }
```

### 2. Ambil Semua Data User (Read All)
Menampilkan daftar seluruh user yang ada di dalam *database*.

* URL: /api/users
* Method: GET
* Success Response (200 OK):
```json
    {
        "status": "success",
        "data": [
            {
                "id": "24f2da67-4c21-4c8b-b952-b8aa93d2eb03",
                "name": "Hitam Legam",
                "age": 25
            }
        ]
    }
```

### 3. Ambil Detail User Spesifik (Read Detail)
Mencari dan menampilkan detail satu user berdasarkan ID.

* URL: /api/users/{id}
* Method: GET
* URL Params: id=[String]
* Success Response (200 OK):
```json
    {
        "status": "success",
        "data": {
            "id": "24f2da67-4c21-4c8b-b952-b8aa93d2eb03",
            "name": "Hitam Legam",
            "age": 25
        }
    }
```

### 4. Ubah Data User (Update)
Memperbarui data nama dan/atau umur dari user yang sudah ada.

* URL: /api/users/{id}
* Method: PUT
* URL Params: id=[String]
* Request Body:
```json
    {
        "name": "Hitam Glosy",
        "age": 23
    }
    
* Success Response (200 OK):
    json
    {
        "status": "success",
        "data": {
            "id": "24f2da67-4c21-4c8b-b952-b8aa93d2eb03",
            "name": "Hitam Glosy",
            "age": 23
        }
    }
``` 

### 5. Hapus Data User (Delete)
Menghapus data user secara permanen dari *database*.

* URL: /api/users/{id}
* Method: DELETE
* URL Params: id=[String]
* Success Response (200 OK):
```json
    {
        "status": "success delete user with id 24f2da67-4c21-4c8b-b952-b8aa93d2eb03"
    }
```

### ScreenShoot web nya
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/d925138a-9000-4266-9f4b-dc2bc28325ff" />
