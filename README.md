# grade-management-system

Database Details:
********************
Schema: 
---------
grade_management_system

Tables:
----------
student_teacher_registration

Commands:
---------
mysql> show databases;

mysql> use grade_management_system;

mysql> show tables;

mysql> select * from  student_teacher_registration;



Ports:
-------------
student-teacher-login-service : 8080
student-teacher-registration-service : 8081
student-teacher-profile-update-service: 8082
student-teacher-forgot-password-service : 8083
student-teacher-marks-data-service : 8084
student-details-service: 8085
student-teacher-eureka-server : 8761
student-teacher-zuul-api : 8765
student-teacher-cloud-config-server : 8888

End points:
----------------
Eureka: http://localhost/8761

Registration:
-----------------------
Forgot Password: http://localhost:8081/reg/password/v1/updatePassword

Update Profile: http://localhost:8081/reg/profile/v1/updateProfile

Authenticate: http://localhost:8081/reg/login/v1/authenticate

Register: http://localhost:8081/registration/v1/saveCustomer

Marks Data Service:
---------------------------
Update Marks: http://localhost:8084/marks/v1/updateMarks

Get Marks By Id: http://localhost:8084/marks/v1/getMarksById

All Students Details Service:
-------------------------------
Get All Student Details: http://localhost:8085/student/details/v1/getAllStudentDetails

Requests Via API Gate Way
*****************************
Forgot Password: http://localhost:8765/student-teacher-forgot-password-service/forgot/v1/updatePassword

Update Profile: http://localhost:8765/student-teacher-profile-update-service/profile/v1/updateProfile

Get Profile By Id: http://localhost:8765/student-teacher-profile-update-service/profile/v1/getProfileById

Authenticate: http://localhost:8765/student-teacher-login-service/login/v1/authenticate

Update Marks: http://localhost:8765/student-teacher-marks-data-service/marks/v1/updateMarks

Get Marks By Id: http://localhost:8765/student-teacher-marks-data-service/marks/v1/getMarksById

Register Customer: http://localhost:8765/student-teacher-registration-service/registration/v1/saveCustomer
