This repo aims to turn your RPI into a server with deployed api inside.

to start your api we will use gunicorn 

```
pip3 install gunicorn
```


you can start the basicAPI.py with 

```
gunicorn --bind 0.0.0.0:5000 basicAPI:app
```

how it works 

`gunicorn` is the green unicorn web server it runs your flask python api

`--bind` to select address 

`0.0.0.0` to bind to all available network interfaces

`:5000` our flask runs on  port 5000 so make gunicorn listen it


`basicAPI:app` run the app defined inside basicAPI.py file


To test your api locally go this address

```
http://127.0.0.1:5000
```
or 
```
http://localhost:5000
```

to close safely you can close with

```
sudo pkill gunicorn
```