# Abacus-Class-Record

Abacus is the visual platform that gives teachers perspective on class attendances, assignments, and grades.

A working version of the application can be found at [https://react-abacus.herokuapp.com](https://react-abacus.herokuapp.com "ABACUS CLASS RECORD, made with React")

---

## Motivation for Development

- Teachers need one place, a reliable database, to digitally track all of their critical information.

- Abacus aims to provide teachers with a way to clearly visualize their analytics and provide at-a-glance insights into what's going on in their classes.

---

## How This App Works

### Display all the classrooms in the database
![Get all classrooms](https://i.imgur.com/VJSc88c.png)

### Check in students and display attendance overview
![Attendance ](https://i.imgur.com/XrXYy1u.png)

### Filter assignments by type and add files to each assignment
![Assignments ](https://i.imgur.com/ljDmlxf.png)

### Add grades by assignment
![Grades ](https://i.imgur.com/6yAC6qp.png)

---

## Technologies used

### Front-End

- `Create-React-App`
- `React Developer Tools`
- `React-Datepicker`
- `Moment`
- `Axios`
- `Joi-Browser`
- `JWT-Decode`

### Back-End

- `Node.js`
- `Express`
- `MongoDb`
- `Mongoose`
- `Joi`
- `Bcrypt`
- `JSON Web Tokens`

---

## RESTful API Services

### User Creation and Authentication

| Route      | HTTP Verb | Description   |
| ---------- | --------- | ------------- |
| /api/users | `POST`    | Create a user |
| /api/auth  | `POST`    | Login a user  |

### Classrooms

| Route                         | HTTP Verb | Description                      |
| ----------------------------- | --------- | -------------------------------- |
| /api/classrooms               | `GET`     | Get all the classrooms           |
| /api/classrooms               | `POST`    | Create a classroom               |
| /api/classrooms/:classroom_id | `GET`     | Get a single classroom           |
| /api/classrooms/:classroom_id | `PUT`     | Update a classroom with new info |
| /api/classrooms/:classroom_id | `DELETE`  | Delete a classroom               |

### Teachers

| Route                     | HTTP Verb | Description                    |
| ------------------------- | --------- | ------------------------------ |
| /api/teachers             | `GET`     | Get all the teachers           |
| /api/teachers             | `POST`    | Create a teacher               |
| /api/teachers/:student_id | `GET`     | Get a single teacher           |
| /api/teachers/:student_id | `PUT`     | Update a teacher with new info |
| /api/teachers/:student_id | `DELETE`  | Delete a teacher               |

### Students

| Route                     | HTTP Verb | Description                    |
| ------------------------- | --------- | ------------------------------ |
| /api/students             | `GET`     | Get all the students           |
| /api/students             | `POST`    | Create a student               |
| /api/students/:student_id | `GET`     | Get a single student           |
| /api/students/:student_id | `PUT`     | Update a student with new info |
| /api/students/:student_id | `DELETE`  | Delete a student               |

### Attendance

| Route                                              | HTTP Verb | Description                     |
| -------------------------------------------------- | --------- | ------------------------------- |
| /api/attendance/:classroom_id/:class_date          | `GET`     | Get attendance                  |
| /api/attendance                                    | `POST`    | Crete attendance                |
| /api/attendance/:attendance_id                     | `PUT`     | Check in or check out a student |
| /api/attendance/checkin/:classroom_id/:class_date  | `PUT`     | Check in all students           |
| /api/attendance/checkout/:classroom_id/:class_date | `PUT`     | Check out all students          |
| /api/attendance/:attendance_id                     | `DELETE`  | Delete attendance               |
|                                                    |

### Assignments

| Route                                | HTTP Verb | Description                          |
| ------------------------------------ | --------- | ------------------------------------ |
| /api/assignments/view/:assignment_id | `GET`     | Get an assignment                    |
| /api/assignments/:classroom_id       | `GET`     | Get all assignments in a given class |
| /api/assignments                     | `POST`    | Create an assignment                 |
| /api/assignments/:assignment_id      | `DELETE`  | Delete an assignment                 |

### Grades

| Route                                 | HTTP Verb | Description                                           |
| ------------------------------------- | --------- | ----------------------------------------------------- |
| /api/grades/:grade_id                 | `GET`     | Get grade of a student                                |
| /api/grades/assignment/:assignment_id | `GET`     | Get all grades of a certain assignment                |
| /api/grades/student/:student_id       | `GET`     | Get all grades of a certain student                   |
| /api/grades                           | `POST`    | Create grade with a classroom id and an assignment id |
| /api/grades/:grade_id                 | `PUT`     | Update grade with new info                            |
| /api/grades/:grade_id                 | `DELETE`  | Delete grade                                          |

---
## Authors
**Abacus Inc. Team Members**
* [Victor Adams](https://kysper.github.io/)
* [Reed Kroh](https://github.com/reedkroh)
* [Andrew Ulm](https://github.com/andrewulm)
* [Keen Wilson](https://keenwilson.com)

_This product is part of the Full-Stack Web Development program at University of Kansas_

