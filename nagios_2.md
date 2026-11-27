docker pull jasonrivers/nagios:latest

docker run --name nagiosdemo -p 8888:80 jasonrivers/nagios:latest

go to browser and http://localhost:8888

username: nagiosadmin
password: nagios

open another powershell in admin mode

docker ps
docker stop nagiosdemo
docker rm nagiosdemo
