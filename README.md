<p align="center">
  <img src="/gif/sanic.gif"/>
</p>

<h1 align="center"> 🐍 Rinha de Backend 🐍 </h1>
<p align="center"><a href="https://github.com/zanfranceschi/rinha-de-backend-2023-q3">repositório da competicação</a></p>

This project was inspired by a community driven challenge that can be found <a href="https://github.com/zanfranceschi/rinha-de-backend-2023-q3">here</a>.   
The main challenge idea is not the api itself, but the optimization to handle a stress test close to a ddos, using only 1.5 vCPU and 3GB of RAM.   
This version does not attempt to be a production like code and does not apply much of good design standards, everything like that are a completely overengineering to the challenge propose.   
The main features applied to increase performance was:   

- background task queue and bulk insert.   
- cache for people queries.   
- searcheable generated column and trigram index for 'like' query.   
- unix socket connection between nginx and api's nodes.   

it reached 21' position at challenge and 1' made in python.   

Stack:   
- Python
- Sanic
- PostgreSQL
- Redis
- Nginx
