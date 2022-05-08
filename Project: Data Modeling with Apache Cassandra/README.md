## Project description

This Udacity Data Engineering nanodegree project creates an Apache Cassandra database sparkifyks for a music app, Sparkify. The purpose of the NoSQL database is to answer queries on song play data. The data model includes a table for each of the following queries:

1. Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4

2. Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182

3. Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

## Design, File Explanation

The project is located in `Project_1B.ipynb` and files located in `event_data/`

The notebook creates a csv file and uses ETL to create tables and query for the information listed in the above three problems.

## How To Run the Project 

Borrowed Dockerfile information
https://github.com/kenhanscombe/project-cassandra

Run cassandra

```
docker pull cassandra

docker run --name cassandra-container -p 9042:9042 -d cassandra:latest
```

Close and delete the instance 

```
docker stop cassandra-container
docker rm cassandra-container
```