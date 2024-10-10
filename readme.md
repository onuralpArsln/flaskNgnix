This repo aims to turn your RPI into a server with deployed api inside.

to start your api we will use gunicorn 

```
pip3 install gunicorn
```


you can start the basicAPI.py with 

```
gunicorn --bind 0.0.0.0:5000 app:app
```

