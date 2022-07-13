# firebreak-mood-tracker-backend-cf-deployment
## To run: 
Start up a virtual environment. I use pipenv.
### `cp sample.env backend/.env`
Change the environment variables accordingly.
### `pipenv shell`
### `pipenv install`
### `python manage.py migrate`
### `python manage.py run server`

## To deploy:
### Set environment variables with `cf set-env <APP_NAME> <VARIABLE_NAME> <VARIABLE_VALUE>`
This can be a bit tedious if you have lots of variables but not sure how else to get cf to see them.
### `cf push <APP_NAME>`
