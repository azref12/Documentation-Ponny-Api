### *POST* Method
````
[POST] url/job/jobtransaction/
````
`json` :
````
{
    "iduser" : 7, // integer
    "idclient" : 1, // integer
    "no_app" : " ", // integer
    "nama_nasabah" : " ", // string
    "zip_area" : "16350", // string
    "file_pendukung" : [], //JSON
    "image" : [], //JSON
    "surveyor" : " ", // string
    "checker" : " ", // string
    "priority" : 1, // integer
    "status" : 1, // integer
    "remark" : "", // string
    "idtemplate" : 1, // integer
    "data" : 1, // integer
    "service" : 1, // integer
    "alamat_nasabah" : " ", // string
    "kantor" : " ", // string
    "alamat_kantor" : " ", // string
    "zip_area_kantor" : " ", // string
    "jabatan" : " ", // string
    "tanggal" : " ", // string ex: "2024-08-14"
    "limit" : " ", //optional (if null = without date_limit, if "2024-08-31" = with date_limit
    "notes": " " // string
}
````

### *GET* Method
`params` : `idclient`, `tanggal_mulai`, `tanggal_akhir`, `service`, `status`.

````
[GET] url/job/filterjob/?idclient=&tanggal_mulai=2024-07-10&tanggal_akhir=2024-07-12&service=&status=
````

### *PUT* Method

#### Survey
````
[PUT] url/job/jobreadysurveysubmit/
````
`json` :
````
{
    "id" : 1, //id job => integer
    "iduser" : 49, //integer
    "result" : ["lorem ipsum"], //json
    "submit" : 1, //integer
    "image" : [["http://192.168.18.12:8888/bottle.png"]], //json
    "surveyor" :"ADM004" //string
}
````

#### Status Survey
````
[PUT] url/job/jobschangechacker/
````
`json` :
````
{
    "id" : 1, //id job => integer
    "iduser" : 49, //integer
    "checker" : "ADM003" //string
}
````

#### Send Survey
````
[PUT] url/job/jobschangemail/
````
`json` :
````
{
    "id" : 1,
    "iduser" : 49
}
````

