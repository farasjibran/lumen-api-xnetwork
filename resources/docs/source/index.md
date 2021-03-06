---
title: API Reference

language_tabs:
- bash
- javascript

includes:

search: true

toc_footers:
- <a href='http://github.com/mpociot/documentarian'>Documentation Powered by Documentarian</a>
---
<!-- START_INFO -->
# Info

Welcome to the generated API reference.
[Get Postman Collection](http://localhost/docs/collection.json)

<!-- END_INFO -->

#general


<!-- START_d7aad7b5ac127700500280d511a3db01 -->
## register
> Example request:

```bash
curl -X POST \
    "http://localhost/register" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/register"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "POST",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`POST register`


<!-- END_d7aad7b5ac127700500280d511a3db01 -->

<!-- START_ba35aa39474cb98cfb31829e70eb8b74 -->
## login
> Example request:

```bash
curl -X POST \
    "http://localhost/login" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/login"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "POST",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`POST login`


<!-- END_ba35aa39474cb98cfb31829e70eb8b74 -->

<!-- START_568bd749946744d2753eaad6cfad5db6 -->
## logout
> Example request:

```bash
curl -X GET \
    -G "http://localhost/logout" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/logout"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (500):

```json
null
```

### HTTP Request
`GET logout`


<!-- END_568bd749946744d2753eaad6cfad5db6 -->

<!-- START_527c8680c9573c56ec7522dbab123d96 -->
## user/update/{id}
> Example request:

```bash
curl -X POST \
    "http://localhost/user/update/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/user/update/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "POST",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`POST user/update/{id}`


<!-- END_527c8680c9573c56ec7522dbab123d96 -->

<!-- START_8ff3735f0ff86d908093a1d3715c080b -->
## user/get/{id}
> Example request:

```bash
curl -X GET \
    -G "http://localhost/user/get/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/user/get/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "User Detail",
    "data": {
        "id": 1,
        "username": "Admin",
        "email": "admin@admin.com",
        "gambar_user": "http:\/\/localhost:8000\/upload\/user\/U-1610070419.png",
        "created_at": "2021-01-07T08:05:37.000000Z",
        "updated_at": "2021-01-11T06:56:48.000000Z"
    }
}
```

### HTTP Request
`GET user/get/{id}`


<!-- END_8ff3735f0ff86d908093a1d3715c080b -->

<!-- START_b63c55c4bd1dca269829c5efb74328c8 -->
## product
> Example request:

```bash
curl -X GET \
    -G "http://localhost/product" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/product"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "All Product",
    "result": []
}
```

### HTTP Request
`GET product`


<!-- END_b63c55c4bd1dca269829c5efb74328c8 -->

<!-- START_08bbb327768b1f76643752a24a22bde2 -->
## product/store
> Example request:

```bash
curl -X POST \
    "http://localhost/product/store" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/product/store"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "POST",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`POST product/store`


<!-- END_08bbb327768b1f76643752a24a22bde2 -->

<!-- START_b0d7a60af6a41929695b88f946478489 -->
## product/get/{id}
> Example request:

```bash
curl -X GET \
    -G "http://localhost/product/get/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/product/get/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "Product Detail",
    "data": null
}
```

### HTTP Request
`GET product/get/{id}`


<!-- END_b0d7a60af6a41929695b88f946478489 -->

<!-- START_ea844ada583f891e417ad7a1417291d6 -->
## product/update/{id}
> Example request:

```bash
curl -X POST \
    "http://localhost/product/update/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/product/update/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "POST",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`POST product/update/{id}`


<!-- END_ea844ada583f891e417ad7a1417291d6 -->

<!-- START_3831c107059ee01916385908b4f3df24 -->
## product/delete/{id}
> Example request:

```bash
curl -X DELETE \
    "http://localhost/product/delete/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/product/delete/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "DELETE",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`DELETE product/delete/{id}`


<!-- END_3831c107059ee01916385908b4f3df24 -->

<!-- START_679ea4e19d49028fd5a7bd6ee9f0f308 -->
## contact
> Example request:

```bash
curl -X GET \
    -G "http://localhost/contact" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/contact"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "All Contact",
    "result": {
        "current_page": 1,
        "data": [
            {
                "id": 1,
                "name": "faras",
                "email": "faras@gmail.com",
                "message": "mantep banget banget",
                "created_at": "2021-01-07T08:09:14.000000Z",
                "updated_at": "2021-01-07T08:09:14.000000Z"
            }
        ],
        "first_page_url": "http:\/\/localhost?page=1",
        "from": 1,
        "last_page": 1,
        "last_page_url": "http:\/\/localhost?page=1",
        "next_page_url": null,
        "path": "http:\/\/localhost",
        "per_page": 5,
        "prev_page_url": null,
        "to": 1,
        "total": 1
    }
}
```

### HTTP Request
`GET contact`


<!-- END_679ea4e19d49028fd5a7bd6ee9f0f308 -->

<!-- START_c3e63ee1634dbce422c80cb6e4bba831 -->
## contact/all
> Example request:

```bash
curl -X GET \
    -G "http://localhost/contact/all" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/contact/all"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "All Contact",
    "result": [
        {
            "id": 1,
            "name": "faras",
            "email": "faras@gmail.com",
            "message": "mantep banget banget",
            "created_at": "2021-01-07T08:09:14.000000Z",
            "updated_at": "2021-01-07T08:09:14.000000Z"
        }
    ]
}
```

### HTTP Request
`GET contact/all`


<!-- END_c3e63ee1634dbce422c80cb6e4bba831 -->

<!-- START_1fd7b097be3289adace222522f7231b2 -->
## contact/store
> Example request:

```bash
curl -X POST \
    "http://localhost/contact/store" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/contact/store"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "POST",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`POST contact/store`


<!-- END_1fd7b097be3289adace222522f7231b2 -->

<!-- START_19c7600eeaddf584b3db9bd6cf1c5a81 -->
## contact/get/{id}
> Example request:

```bash
curl -X GET \
    -G "http://localhost/contact/get/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/contact/get/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "Contact Detail",
    "data": {
        "id": 1,
        "name": "faras",
        "email": "faras@gmail.com",
        "message": "mantep banget banget",
        "created_at": "2021-01-07T08:09:14.000000Z",
        "updated_at": "2021-01-07T08:09:14.000000Z"
    }
}
```

### HTTP Request
`GET contact/get/{id}`


<!-- END_19c7600eeaddf584b3db9bd6cf1c5a81 -->

<!-- START_564b242454c7dba1b0557623edf415d8 -->
## contact/update/{id}
> Example request:

```bash
curl -X PUT \
    "http://localhost/contact/update/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/contact/update/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "PUT",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`PUT contact/update/{id}`


<!-- END_564b242454c7dba1b0557623edf415d8 -->

<!-- START_81218d0f6ec3dd19d6c3b6363c2b9054 -->
## contact/delete/{id}
> Example request:

```bash
curl -X DELETE \
    "http://localhost/contact/delete/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/contact/delete/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "DELETE",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`DELETE contact/delete/{id}`


<!-- END_81218d0f6ec3dd19d6c3b6363c2b9054 -->

<!-- START_639ac0e7925863599ff4bac54d3ec452 -->
## contact/count
> Example request:

```bash
curl -X GET \
    -G "http://localhost/contact/count" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/contact/count"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "All Contact",
    "result": 0
}
```

### HTTP Request
`GET contact/count`


<!-- END_639ac0e7925863599ff4bac54d3ec452 -->
<!-- START_46b1e33f1f220f54df51acd2635a5c0f -->
## job
> Example request:

```bash
curl -X GET \
    -G "http://localhost/job" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/job"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "All Job",
    "result": [
        {
            "id": 2,
            "job_position": "General Manager (GM)",
            "job_location": "Jakarta Timur",
            "job_description": "Dibutuhkan general manager dengan pendidikan minimal S1",
            "job_link": "www.facebook.com",
            "created_at": "2021-01-07T09:08:20.000000Z",
            "updated_at": "2021-01-07T09:08:20.000000Z"
        }
    ]
}
```

### HTTP Request
`GET job`


<!-- END_46b1e33f1f220f54df51acd2635a5c0f -->

<!-- START_75390186a7878f8dd243bfd5f810ecde -->
## job/store
> Example request:

```bash
curl -X POST \
    "http://localhost/job/store" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/job/store"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "POST",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`POST job/store`


<!-- END_75390186a7878f8dd243bfd5f810ecde -->

<!-- START_89acfa202f5a8ca3a7560059c19698d6 -->
## job/get/{id}
> Example request:

```bash
curl -X GET \
    -G "http://localhost/job/get/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/job/get/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "Job Detail",
    "data": null
}
```

### HTTP Request
`GET job/get/{id}`


<!-- END_89acfa202f5a8ca3a7560059c19698d6 -->

<!-- START_c7619996c81f50a57f09ccaf4cb615a2 -->
## job/update/{id}
> Example request:

```bash
curl -X PUT \
    "http://localhost/job/update/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/job/update/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "PUT",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`PUT job/update/{id}`


<!-- END_c7619996c81f50a57f09ccaf4cb615a2 -->

<!-- START_dd0aa004902547e2e1bc2542228d4dec -->
## job/delete/{id}
> Example request:

```bash
curl -X DELETE \
    "http://localhost/job/delete/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/job/delete/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "DELETE",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`DELETE job/delete/{id}`


<!-- END_dd0aa004902547e2e1bc2542228d4dec -->

<!-- START_31a54f5500ada6b023a98d4c592dd6eb -->
## radio
> Example request:

```bash
curl -X GET \
    -G "http://localhost/radio" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/radio"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "All Radio",
    "result": [
        {
            "id": 7,
            "fm_channel": "105.5FM",
            "kota": "KABUPATEN ACEH SINGKIL",
            "created_at": "2021-01-11T03:14:18.000000Z",
            "updated_at": "2021-01-11T03:14:18.000000Z"
        }
    ]
}
```

### HTTP Request
`GET radio`


<!-- END_31a54f5500ada6b023a98d4c592dd6eb -->

<!-- START_be677216fbf4029725dba734cab7aca1 -->
## radio/store
> Example request:

```bash
curl -X POST \
    "http://localhost/radio/store" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/radio/store"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "POST",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`POST radio/store`


<!-- END_be677216fbf4029725dba734cab7aca1 -->

<!-- START_ef5fbfe9fc661244314cda8e7b23fdc1 -->
## radio/get/{id}
> Example request:

```bash
curl -X GET \
    -G "http://localhost/radio/get/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/radio/get/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "Radio Detail",
    "data": null
}
```

### HTTP Request
`GET radio/get/{id}`


<!-- END_ef5fbfe9fc661244314cda8e7b23fdc1 -->

<!-- START_11c5da352031eb4e5a1a45d04129d0db -->
## radio/update/{id}
> Example request:

```bash
curl -X PUT \
    "http://localhost/radio/update/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/radio/update/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "PUT",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`PUT radio/update/{id}`


<!-- END_11c5da352031eb4e5a1a45d04129d0db -->

<!-- START_3d347f3aba958a484a66d3d943b814ea -->
## radio/delete/{id}
> Example request:

```bash
curl -X DELETE \
    "http://localhost/radio/delete/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/radio/delete/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "DELETE",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`DELETE radio/delete/{id}`


<!-- END_3d347f3aba958a484a66d3d943b814ea -->

<!-- START_67f83cf70c445defc811f2582ac11de5 -->
## radiocoverage
> Example request:

```bash
curl -X GET \
    -G "http://localhost/radiocoverage" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/radiocoverage"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "All RadioCoverage",
    "result": [
        {
            "id": 4,
            "provinsi": "ACEH",
            "kota": "KABUPATEN ACEH SINGKIL",
            "stasiun_id": "Kaneka",
            "fm": "105.5FM",
            "created_at": "2021-01-11T03:14:44.000000Z",
            "updated_at": "2021-01-11T03:14:44.000000Z"
        }
    ]
}
```

### HTTP Request
`GET radiocoverage`


<!-- END_67f83cf70c445defc811f2582ac11de5 -->

<!-- START_0e8c7c21822fc3226565ebfeb28211e8 -->
## radiocoverage/store
> Example request:

```bash
curl -X POST \
    "http://localhost/radiocoverage/store" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/radiocoverage/store"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "POST",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`POST radiocoverage/store`


<!-- END_0e8c7c21822fc3226565ebfeb28211e8 -->

<!-- START_78f5dae0ab5923f656057978ce34e195 -->
## radiocoverage/get/{id}
> Example request:

```bash
curl -X GET \
    -G "http://localhost/radiocoverage/get/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/radiocoverage/get/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "RadioCoverage Detail",
    "data": null
}
```

### HTTP Request
`GET radiocoverage/get/{id}`


<!-- END_78f5dae0ab5923f656057978ce34e195 -->

<!-- START_9345daa47aa5f9347adfe58e11cdaa81 -->
## radiocoverage/update/{id}
> Example request:

```bash
curl -X PUT \
    "http://localhost/radiocoverage/update/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/radiocoverage/update/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "PUT",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`PUT radiocoverage/update/{id}`


<!-- END_9345daa47aa5f9347adfe58e11cdaa81 -->

<!-- START_1e55aff5294073935fc12e5c2e787580 -->
## radiocoverage/delete/{id}
> Example request:

```bash
curl -X DELETE \
    "http://localhost/radiocoverage/delete/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/radiocoverage/delete/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "DELETE",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`DELETE radiocoverage/delete/{id}`


<!-- END_1e55aff5294073935fc12e5c2e787580 -->

<!-- START_e227f17e1cc2d345b8b679b7ab7e49b4 -->
## printradio/{provinsi}
> Example request:

```bash
curl -X GET \
    -G "http://localhost/printradio/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/printradio/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "Data Report Pdf"
}
```

### HTTP Request
`GET printradio/{provinsi}`


<!-- END_e227f17e1cc2d345b8b679b7ab7e49b4 -->

<!-- START_3bcedda78ae45ef5c0f4c97a4963b7a1 -->
## user
> Example request:

```bash
curl -X GET \
    -G "http://localhost/user" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/user"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "GET",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```


> Example response (200):

```json
{
    "success": true,
    "status": 200,
    "message": "All User",
    "result": [
        {
            "id": 1,
            "username": "Admin",
            "email": "admin@admin.com",
            "gambar_user": "http:\/\/localhost:8000\/upload\/user\/U-1610070419.png",
            "created_at": "2021-01-07T08:05:37.000000Z",
            "updated_at": "2021-01-11T06:56:48.000000Z"
        }
    ]
}
```

### HTTP Request
`GET user`


<!-- END_3bcedda78ae45ef5c0f4c97a4963b7a1 -->

<!-- START_844f41533384ba37d114c7189b6df5d0 -->
## user/store
> Example request:

```bash
curl -X POST \
    "http://localhost/user/store" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/user/store"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "POST",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`POST user/store`


<!-- END_844f41533384ba37d114c7189b6df5d0 -->

<!-- START_e4848f0937afe29d1f4ba623c0d6925d -->
## userupdate/{id}
> Example request:

```bash
curl -X PUT \
    "http://localhost/userupdate/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/userupdate/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "PUT",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`PUT userupdate/{id}`


<!-- END_e4848f0937afe29d1f4ba623c0d6925d -->

<!-- START_76f053a055f8b5067f748a14c19ef101 -->
## user/delete/{id}
> Example request:

```bash
curl -X DELETE \
    "http://localhost/user/delete/1" \
    -H "Content-Type: application/json" \
    -H "Accept: application/json"
```

```javascript
const url = new URL(
    "http://localhost/user/delete/1"
);

let headers = {
    "Content-Type": "application/json",
    "Accept": "application/json",
};

fetch(url, {
    method: "DELETE",
    headers: headers,
})
    .then(response => response.json())
    .then(json => console.log(json));
```



### HTTP Request
`DELETE user/delete/{id}`


<!-- END_76f053a055f8b5067f748a14c19ef101 -->


