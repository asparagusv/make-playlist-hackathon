

https://github.com/asparagusv/make-playlist-hackathon/assets/41145723/1dd0fb55-5627-4f3f-8742-1c06d987029f

![1_3 1 1](https://github.com/asparagusv/make-playlist-hackathon/assets/41145723/ce36571a-41f8-49e5-bc05-8e09a4122406)
![2_3 1 2](https://github.com/asparagusv/make-playlist-hackathon/assets/41145723/dfe12640-a72c-460d-aa19-305abe36a0b3)
![3_3 2 1](https://github.com/asparagusv/make-playlist-hackathon/assets/41145723/bd186064-4f25-4de6-b7de-349890945cae)
![4_3 2 2](https://github.com/asparagusv/make-playlist-hackathon/assets/41145723/5ced6dc2-9507-4307-93a6-ae0a11ace1e1)
![5_3 2 3](https://github.com/asparagusv/make-playlist-hackathon/assets/41145723/1eeb6edc-4750-47cf-beb3-1df58c5251cd)
![6_3 4 1](https://github.com/asparagusv/make-playlist-hackathon/assets/41145723/d5014785-59af-428c-adf1-4336e4c0ad33)


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
