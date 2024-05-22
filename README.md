# aws
### Install Web Server
```
sudo yum install httpd 
sudo systemctl start httpd
sudo systemctl enable httpd
```
```
sudo vi /var/www/html/index.html
<!DOCTYPE html>
<html>
  <head>
    <title>Apache Web Server</title>
  </head>
  <body>
    <h1>Apache Web Server</h1>
    <p>This is a simple HTML web page.</p>
  </body>
</html>
```
### Install Python Flask App
```
pip3 install flask
python3 app.py
python3 -m flask --app board run --port 8000 --host 0.0.0.0 --debug
```
