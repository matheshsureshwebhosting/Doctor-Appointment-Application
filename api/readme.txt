doctors
---------
POST => http://localhost:4000/doctor/add

header -> nill

body -> 
{
	       "doctor_name": "Jhon",
            "doctor_hospital": "ABC Hospital",
            "doctor_description": "Eye Care",
            "doctor_email": "jhon@gmail.com",
            "doctor_mobile": "917845869542",
            "doctor_address": "123,abc,xyz-61"
}

GET => http://localhost:4000/doctor/viewall

GET  => http://localhost:4000/editdoctor/view

header -> 
doctor_id 77c5f75a-76e5-47d0-bdf3-78da4ee9f38c

slot
-----------
POST => http://localhost:4000/slot/create

header -> 

doctor_id 77c5f75a-76e5-47d0-bdf3-78da4ee9f38c

body -> 
{
	"date":"2021-05-16", 
	"startingTime":"10:00", 
	"endingTime":"15:00", 
	"duration":"30"
}

POST => http://localhost:4000/slot/view
header -> 
doctor_id 77c5f75a-76e5-47d0-bdf3-78da4ee9f38c

body -> 
{
	"date":"2021-05-16", 
}


patient
--------------
POST => http://localhost:4000/user/siginup
header-> nill

body ->
{
	 "pname": "Max",
            "pemail": "max@gmail.com",
            "pnumber": "042256587",
            "password": "max@gmail.com",
            "pdob": "1978-05-15",
            "page":"48"
}

appointment
-----------------

POST => http://localhost:4000/appoinment
header-> 
doctor_id  77c5f75a-76e5-47d0-bdf3-78da4ee9f38c
puserid    fd5a82ac-a14d-4b82-85f9-a356206dbf6d

body ->
{
	"slot":"slot_2",
	"date":"2021-05-16"
}

