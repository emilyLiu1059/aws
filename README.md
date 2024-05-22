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
```
sudo yum install python3-devel

pip3 install flask_mysqldb
   73  mysql_config
   74  udo yum install mysql-devel gcc gcc-devel python-devel
   75  sudo yum install mysql-devel gcc gcc-devel python-devel
   76  pip3 install flask_mysqldb
   77  pip install mysql-connector-python
   78  pip3 install mysql-connector-python
   79  ls -tlr
   80  python3 app.py
   81  sudo easy_install mysql-python
   82  python3 app.py
   83  pip3 install flask_mysqldb
   84  sudo yum install python3-devel
   85  pip3 install flask_mysqldb
```

```
from flask import Flask

app = Flask(__name__)

@app.route("/")
def hello_world():
    return "<p>Hello, World!</p>"
if __name__ == "__main__":
    app.run(host="0.0.0.0", port=8000, debug=True)
```

