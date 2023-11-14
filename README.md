https://github.com/asparagusv/make-playlist-hackathon/assets/41145723/52fcbe1d-948b-474f-b211-ad3f664fba7a


#Mac/Linux

terminal 1
```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
export SPOTIPY_CLIENT_ID=insert_your_client_id_here
export SPOTIPY_CLIENT_SECRET=insert_your_client_secret_here
export SPOTIPY_REDIRECT_URI='http://127.0.0.1:8080'
sudo service redis-server start
```

terminal 2
```
venv/bin/celery -A app.celery worker --loglevel=DEBUG
```

terminal 1
```
venv/bin/python app.py
```

ref  
<https://github.com/miguelgrinberg/flask-celery-example>  
<https://redis.io/docs/install/install-redis/install-redis-on-windows/>
