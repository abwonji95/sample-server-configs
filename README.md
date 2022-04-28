# sample-server-configs


This repo is for detailed instruction on creating various configs for heroku server and IIS server .

languages   


#1 . Angular -Front-end , 

#2 . Django -Backend,

#3 . Node-Js -Server-side


Steps Deploying Django application on Heroku.

`Pip install whitenoise `

`Pip install gunicorn `

Remember to add them to `Settings.py`

Add ` STATIC_ROOT=os.path.join(BASE_DIR, 'static')`  to `Settings.py`

Add `'whitenoise.middleware.WhiteNoiseMiddleware',` Middleware to `Settings.py`


