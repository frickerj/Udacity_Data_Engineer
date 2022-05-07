## Project description

This Udacity Data Engineering nanodegree project creates a postgres database `sparkifydb` for a music app, Sparkify. The purpose of the database is to model song and log datasets (originaly stored in JSON format) with a star schema optimised for queries on song play analysis

## Database design

![erd_image.png]

## ETL Process



## Project Repository files

`sql_queries.py` contains the sql queries that are run as part of `etl.py`

`create_tables.py` is run first, this creates the tables for the project. 

## How To Run the Project 

Borrowed Dockerfile postgres and init.sql files from here
https://github.com/kenhanscombe/project-postgres/

To build from Dockerfile and init.sql and run from local build image

```
docker build -t postgres-student-image .

docker run -d --name postgres-student-container -p 5432:5432 postgres-student-image
```