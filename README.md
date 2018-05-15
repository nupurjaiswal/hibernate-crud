# Hibernate Create Read Update Delete Project

- Technologies Used: Spring, Hibernate, MySQL
 
## Steps:
- Execute the SQL script:
 ```sh
CREATE USER 'hbstudent'@'localhost' IDENTIFIED BY 'hbstudent';

GRANT ALL PRIVILEGES ON * . * TO 'hbstudent'@'localhost';

CREATE DATABASE  IF NOT EXISTS `hb_student_tracker`;

USE `hb_student_tracker`;

DROP TABLE IF EXISTS `student`;

CREATE TABLE `student` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `first_name` varchar(45) DEFAULT NULL,
  `last_name` varchar(45) DEFAULT NULL,
  `email` varchar(45) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=latin1;

```

- hibernate-crud/src has the following class to perform basic operations in database using Java:
    1. CreateStudentDemo
    2. DeleteStudentDemo
    3. PrimaryKeyDemo
    4. QueryStudentDemo
    5. ReadStudentDemo
    6. UpdateStudentDemo