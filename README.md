## Student Management Core
Core management service for the Student Management Application.

###  __API__

#### `/professor/courses/student`

`> Request-type:` _POST_

`> Body:`

```json
{
    username: "joedoe",
    course_name: "Analiza Matematica",
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2ODMwMjE1OTIsImN1c3RvbSI6eyJ1c2VybmFtZSI6Im5vdHNvZmluYWxib3NzIiwibmFtZSI6IkZpbmFsIEJvc3MifX0.V4GK6d7HOYoSRvmlehPzH3LFcINXiErEWMLnVzlFO1Q"
}
```

`> Response:`

* __200 OK__
* __400 BAD REQUEST__

#### `/professor/courses`
---
`> Request-type:` _POST_

`> Body:`

```json
{
    course_name: "Analiza Matematica",
    weekday: "Monday",
    start_hour: "10:00",
    end_hour: "12",
    location: "EC105",
    max_students: "120",
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2ODMwMjE1OTIsImN1c3RvbSI6eyJ1c2VybmFtZSI6Im5vdHNvZmluYWxib3NzIiwibmFtZSI6IkZpbmFsIEJvc3MifX0.V4GK6d7HOYoSRvmlehPzH3LFcINXiErEWMLnVzlFO1Q"
}
```
`> Response:`

* __200 OK__
* __400 BAD REQUEST__

#### `/professor/courses/grades`

`> Request-type:` _POST_

```json
{
    username: "joedoe",
    course_name: "Analiza Matematica",
    grade: 10,
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2ODMwMjE1OTIsImN1c3RvbSI6eyJ1c2VybmFtZSI6Im5vdHNvZmluYWxib3NzIiwibmFtZSI6IkZpbmFsIEJvc3MifX0.V4GK6d7HOYoSRvmlehPzH3LFcINXiErEWMLnVzlFO1Q"
}
```

`> Response:`

* __200 OK__
* __400 BAD REQUEST__

#### `/student/grades`

`> Request-type:` _GET_

```json
{
    username: "joedoe",
    course_name: "Analiza Matematica",
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2ODMwMjE1OTIsImN1c3RvbSI6eyJ1c2VybmFtZSI6Im5vdHNvZmluYWxib3NzIiwibmFtZSI6IkZpbmFsIEJvc3MifX0.V4GK6d7HOYoSRvmlehPzH3LFcINXiErEWMLnVzlFO1Q"
}
```

`> Response:`

* __200 OK__
    ```json
    {
        grade: 10
    }
    ```

* __400 BAD REQUEST__

#### `/student/courses`

`> Request-type:` _GET_

```json
{
    username: "joedoe",
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2ODMwMjE1OTIsImN1c3RvbSI6eyJ1c2VybmFtZSI6Im5vdHNvZmluYWxib3NzIiwibmFtZSI6IkZpbmFsIEJvc3MifX0.V4GK6d7HOYoSRvmlehPzH3LFcINXiErEWMLnVzlFO1Q"
}
```

`> Response:`

* __200 OK__
    ```json
    {
        courses: [
            "Analiza Matematica",
            "Algebra Liniara",
            "Programare 1"
        ]
    }
    ```

* __400 BAD REQUEST__
