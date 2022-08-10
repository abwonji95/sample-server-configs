# 33 sample-server-configs


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

Add `ALLOWED_HOSTS=[*webiste@example.com*,*localhost:8000* ]` to `Settings.py`

then Create a `Procfile` sample provided

Finally open  the directory and in the commandline run   `pip freeze > requirements.txt` to generate your required application dependencies.

Thre are 3 ways to deploy on heroku

# 1.Via GitHub Repo
  1.Login to your Heroku Account
  
  2.on the Dashboard click `NEW` then `create new app` name your application ,finnally click `create app`
  
  3.Once redirected click `github connect to github` then click the button `connect to Github` 
  
  4.you will be redirected and promoted to login to your github account.
  
  5. After login ,select the repo you want to deploy

  6. select the branch

  7. choose whether  you want `Automatic Deployment`  or not

  8. Finished. 

# 2. Via Heroku CLI

Prerequiresites :

1.install `Heroku CLI` and `GIT CLI`

2. initialize your repo `git init`

3. then `git add . `

4. then `git commit m "first commmit"`

5. then create heroku remote using `heroku create -a example-app`

6. For existing app in heroku use `heroku git:remote -a example-app`

7.  to rename use git `remote rename heroku app-new-name`

8.  Now you can Deploy using `git push heroku main` or `git push heroku testbranch:main` for 
  other branches except main



