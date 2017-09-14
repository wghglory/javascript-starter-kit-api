# javascript-starter-kit-api

API for <https://github.com/wghglory/javascript-starter-kit>

This api repository will be hosted in Heroku.

## Heroku configuration

* app.json - describe app to Heroku
* Procfile - command that Heroku should run

## Deploy to Heroku

Since app.json tells Heroku our application address. When `Heroku create`, it knows all information about our application.

Heroku create app, and then we add remote for the app. Last, we publish the app

```bash
heroku login
heroku create  # https://agile-thicket-69985.herokuapp.com/ | https://git.heroku.com/agile-thicket-69985.git
heroku git:remote -a agile-thicket-69985
git push heroku master
```

> Any time we changes the api, we commit the change, then git push heroku master. Heroku will take code from github and deploy it to the url.