
## Deployment

Deploy [Flower](https://github.com/mher/flower/) to Heroku to monitor [Celery](http://www.celeryproject.org/).

Configure the app by providing your broker url (RabbitMQ, Redis) and the Google OpenID auth email domain for logging into Flower. Please read the instructions for [enabling Google OAuth](http://flower.readthedocs.io/en/latest/auth.html#google-oauth-2-0).


## Local development

You can copy the configuration down to your environment via:

```shell
heroku config -s -a [your app] > .env
```

Then prefix each line with `export ` and save the file.

To run, activate your virtual environment and source the environment variables (`source .env`)
To run flower:
`heroku local web`

