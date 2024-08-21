### *POST* Method
````
[POST] url/user/register/
````
`json` :
````
{
    "first_name" : "Lorem",
    "last_name" : "Ipsum",
    "username" : "loremm",
    "email" : "loremipsum@gmail.com",
    "password" : "123123123",
    "phone_number" : "+123",
    "status_privasi" : 1,
    "status_aktivasi" : 1,
    "kategori" : 1,
    "alamat" : "Galaxy",
    "url" : [],
    "extradata" : {
        "alamat" : "Galaxy"
    }
}
````

#### Update User Status
````
[POST] url/user/status_user/49
````
`json` :
````
{
    "status_user" : 1
}
````

#### User Login 
````
[POST] url/user/login/
````
`json` :
````
{
    "username" : "anonim",
    "password" : "123123123"
}
````

### *GET* Method
#### All User
````
[POST] url/user/alluser/
````

#### User Details
````
[POST] url/user/user_detail/1
````

### *PUT* Method
#### User Update
````
[PUT] url/user/update_user/44
````
`json` :
````
{
    "email" : "loremipsum@gmail.com",
    "first_name" : "Lorem",
    "last_name" : "Ipsum",
    "phone_number" : "+6281223451234",
    "kategori" : 1,
    "password" : "",
    "url" : ["svy1.jpeg"], 
    "extradata" : {
        "alamat" : ""
    }
}
````

### *DELETE* Method
````
[DELETE] url/user/update_user/44
````