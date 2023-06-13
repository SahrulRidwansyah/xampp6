# xampp6

```
Nama  : Sahrul Ridwansyah
kelas : TI.22.A2
Nim   : 312210063
```

kodiangan 
```
CREATE TABLE DEPARTMENT (
    ->   department_id INT PRIMARY KEY,
    ->   department_name VARCHAR(255),
    ->   manager_id INT
    -> );

CREATE TABLE EMPLOYEE (
    ->   employee_id INT PRIMARY KEY,
    ->   employee_name VARCHAR(255),
    ->   department_id INT,
    ->   supervisor_id INT,
    ->   FOREIGN KEY (department_id) REFERENCES DEPARTMENT(department_id),
    ->   FOREIGN KEY (supervisor_id) REFERENCES EMPLOYEE(employee_id)
    -> );
 ```
 ![image](https://github.com/sahrul180304/xampp6/assets/115526901/444e8c3d-6e14-4837-b50d-213f94849730)


![image](https://github.com/sahrul180304/xampp6/assets/115526901/96b08148-1ecb-4a01-aa7b-c81fc983b2c6)


```
CREATE TABLE PROJECT (
    ->   project_id INT PRIMARY KEY,
    ->   project_name VARCHAR(255)
    -> );

 CREATE TABLE EMPLOYEE_PROJECT (
    ->   employee_id INT,
    ->   project_id INT,
    ->   FOREIGN KEY (employee_id) REFERENCES EMPLOYEE(employee_id),
    ->   FOREIGN KEY (project_id) REFERENCES PROJECT(project_id),
    ->   PRIMARY KEY (employee_id, project_id)
    -> );
```
![image](https://github.com/sahrul180304/xampp6/assets/115526901/2e5ab746-ad44-4b6d-b488-0bee2c112bd4)


![image](https://github.com/sahrul180304/xampp6/assets/115526901/f06882a3-0971-404c-8d5b-ce77d7cbb27c)



er-d

![image](https://github.com/sahrul180304/xampp6/assets/115526901/e2b1e348-300e-46ff-8195-2b0a9d5ddef4)



