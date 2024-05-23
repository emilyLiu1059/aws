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
sudo yum install -y mysql-devel gcc python3-devel
pip3 install flask
pip3 install flask_mysqldb
```
```
from flask import Flask
app = Flask(__name__)
@app.route("/")
def hello_world():
    return "<p>Hello, World!</p>"
if __name__ == "__main__":
    app.run(host="0.0.0.0", port=8000, debug=True)

python3 app.py
```
```
python3 -m flask --app board run --port 8000 --host 0.0.0.0 --debug
```

