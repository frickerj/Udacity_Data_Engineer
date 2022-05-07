


Borrowed Dockerfile postgres and init.sql files from here
https://github.com/kenhanscombe/project-postgres/

To build from Dockerfile and init.sql and run from local build image

```
docker build -t postgres-student-image .

docker run -d --name postgres-student-container -p 5432:5432 postgres-student-image
```