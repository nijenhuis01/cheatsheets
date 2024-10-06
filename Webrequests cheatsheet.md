# WEB REQUESTS CHEAT SHEET
## cURL

|Command|Description|
|:---|---|
|curl -s -o example.com/index.tml|Download file|
|curl -k https://inlanefreight.com|Send HEAD request (only prints response headers)|
|curl http://admin:admin@<SERVER_IP>:<PORT>/|Pass HTTP basic authorization credentials in the URL|
|curl -u admin:admin http://<SERVER_IP>:<PORT>/|Set HTTP basic authorization credentials|
|curl -H 'Authorization: Basic YWRtaW46YWRtaW4=' http://<SERVER_IP>:<PORT>/|Set request header|
|curl 'http://<SERVER_IP>:<PORT>/search.php? search=le'|Pass GET parameters|
|curl -X PUT http://<SERVER_IP>:<PORT>/api.php/city/london -d '{"city_name":"New_HTB_City", "country_name":"HTB"}' -H 'Content-Type: application/json'|Send POST request with POST data|
|curl -b 'PHPSESSID=c1nsa6op7vtk7kdis7bcnbadf1' http://<SERVER_IP>:<PORT>/|Set request cookies|
|curl -X POST -d '{"search":"london"}' -H 'Content- Type: application/json' http://<SERVER_IP>: <PORT>/search.php
Send POST request with JSON data|Send POST request with JSON data|

###APIs

|Command|Description|
|:---|---|
|curl http://<SERVER_IP>:<PORT>/api.php/city/london|Read Entry|
|curl -s http://<SERVER_IP>:<PORT>/api.php/city/ | jq|Read all entries|
|curl -X POST http://<SERVER_IP>:<PORT>/api.php/city/ -d '{"city_name":"HTB_City", "country_name":"HTB"}' -H 'Content- Type: application/json'|Create (add)entry|
|curl -X PUT http://<SERVER_IP>:<PORT>/api.php/city/london -d '{"city_name":"New_HTB_City", "country_name":"HTB"}' -H 'Content-Type: application/json'|Update (modify) entry|
|curl -X DELETE http://<SERVER_IP>: <PORT>/api.php/city/New_HTB_City|Delete entry|




	

