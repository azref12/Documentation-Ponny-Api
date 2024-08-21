### *POST* Method
````
[POST] url/client/register/
````
`json` :
````
{
    "iduser" : 49,
    "nama" : "qwerty 3",
    "contact" : "qwerty 3",
    "email" : "qwerty 3",
    "phone_number" : "1",
    "keterangan" : "qwerty 3",
    "email_result" : ["qwerty 3"],
    "idclient" : 1,
    "fee_surveyor" : ["qwerty 3"],
    "fee_checker" : ["qwerty 3"]
}
````

### *GET* Method

#### All Client
````
[GET] url/client/register/
````

#### Client Details 
````
[GET] url/client/registerdetails/8
````

### *PUT* Method 

#### Client
````
[PUT] url/client/registerdetails/8
````
`json` :
````
{
    "iduser" : 49,
    "nama" : "AEON-RUMAH",
    "contact" : "Anonim_1",
    "email" : "anonim_1@gmail.com",
    "phone_number" : "+62123",
    "keterangan" : "qwerty123",
    "email_result" : ["anonim_1@gmail.com"]
}
````

#### Client Status
````
[PUT] url/client/changestatusclient/2
````
`json` :
````
{
    "iduser" : 57,
    "status" : 1
}
````

#### Template
````
[PUT] url/client/client_details/
````
`json` :
````
{   
    "template_client" : [
        {
            "iduser" : 7,
            "id" : 1,
            "idclient" : 1,
            "request" : [{"mode": 1, "field": "Nama", "value": "", "wajib": true, "option": ""}], //json
            "result" : [{"mode": 1, "field": "Nama", "value": "", "wajib": true, "option": ""}] //json
        }
    ]
}
````

