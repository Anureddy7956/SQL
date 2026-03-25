# 📘 Project: Student Management Database
### Step 1 : Open terminal and type (using mysql)
```bash
     sudo mysql 
```
<img width="1914" height="507" alt="image" src="https://github.com/user-attachments/assets/7d3ab718-adf6-439b-b663-fa8e727753be" />

### Step 2: Create Database
```bash
     CREATE DATABASE college;
```
<img width="1920" height="119" alt="image" src="https://github.com/user-attachments/assets/879df8b3-be2e-4fcd-a6b3-c8baa022399d" />

#### check Databases:
```bash
     SHOW DATABASES;
```
<img width="1912" height="377" alt="image" src="https://github.com/user-attachments/assets/5b200532-9f72-4d04-8181-19608e3aca0a" />

#### Use Database 
```bash
     USE college; 
```
<img width="1920" height="78" alt="image" src="https://github.com/user-attachments/assets/89cea0af-921a-4f41-bfd3-426631cb03f9" />

### Step 3 : Create Table 
```bash
   CREATE TABLE student(
   id INT PRIMARY KEY,
   name VARCHAR(20),
   age INT,
   course VARCHAR(20) 
);
```
<img width="1920" height="252" alt="image" src="https://github.com/user-attachments/assets/fff6636c-810a-42e3-af4f-45ff0aa432d5" />

#### Check Table 
```bash
   SHOW TABLES;   
```
<img width="1920" height="256" alt="image" src="https://github.com/user-attachments/assets/60fa6abb-58b4-491b-948d-584d3411377c" />

#### See structure
```bash
   DESCRIBE student;   
```
 <img width="1920" height="364" alt="image" src="https://github.com/user-attachments/assets/801272d5-406c-42ea-bb21-f5855eb44d49" />
    
### Step 4 : Insert the Data
```bash
   INSERT INTO student VALUES(1,'Anya',19,'CSE');

   INSERT INTO student VALUES(2,'Ravi',20,'ECE');

   INSERT INTO student VALUES(3,'Meena',18,'CSE');

   INSERT INTO student VALUES(4,'Kiran',21,'MECH');
```
<img width="1920" height="395" alt="image" src="https://github.com/user-attachments/assets/ec4c2089-3350-414f-9173-5508be6d68b2" />

### Step 5: Display Data
#### Show all records:
```bash
   SELECT * FROM student;
```
<img width="1920" height="357" alt="image" src="https://github.com/user-attachments/assets/e59b8b6c-d7f6-478f-a18c-c7dec3b6845c" />

#### Show only names:
```bash
   SELECT name FROM student;
```
#### Show CSE students:
```bash
   SELECT *FROM student
   WHERE course= 'CSE';
```
### Step 6️⃣ Update Data
#### Change age:
```bash
   UPDATE student
   SET age=22
   WHERE id=4;
```
#### Check:
```bash
   SELECT * FROM student;
```

### Step 7: Delete Data 
### delete student :
```bash
   DELETE FROM student
   WHERE id=2;
```
#### Check:
```bash
   SELECT * FROM student;
```
### Step 8: Extra Queries
#### Sort the data by using age in order  
```bash
   SELECT * FROM student
   ORDER BY age;
```
#### Count students
```bash
   SELECT COUNT(*) FROM student;
```

#### Maximum age 
```bash
   SELECT MAX(age) FROM student;
```
#### Minimum age
```bash
   SELECT MIN(age) FROM student;
```

### Step 9: Drop the Table from the Database
```bash
   DROP TABLE student;
```

