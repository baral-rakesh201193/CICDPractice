FROM ubuntu
 
RUN apt-get update

RUN apt-get install curl

RUN curl https://packages.microsoft.com/keys/microsoft.asc | apt-key add -

RUN rl https://packages.microsoft.com/config/ubuntu/20.04/prod.list | tee /etc/apt/sources.list.d/msprod.list

RUN apt-get install mssql-tools unixodbc-dev -y

RUN apt-get install mssql-server -y
 
