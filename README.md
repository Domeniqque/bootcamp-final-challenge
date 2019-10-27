# Final Challenge - MeetApp

> Rocketseat Bootcamp

After clone this project, **init this modules**.

> git submodule init && git submodule update

## # [API](https://github.com/Domeniqque/gostack-meetup-api) (first)

Install packages on **API** directory

> yarn

Copy `.env.example` to `.env`

> cp .env.example .env

And configure these keys on `.env` file with yours private settings

```bash
## APPLICATION
APP_SECRET=

## MAIL
MAIL_USER=
MAIL_PASS=

## SENTRY
SENTRY_DSN=
```

Install **Docker** and **Docker Compose** to run next comands.

Run migrations to database

> docker-compose run api yarn sequelize db:migrate

Finaly, run the API

> docker-compose up -d

Awesome, your application is available on `http://localhost:3333`.

## # [Web](https://github.com/Domeniqque/gostack-meetup-web)

Make sure **API** and **Reactotron** are available.

Install packages on **web** directory and start the application

> yarn && yarn start

All right, your application is available on `http://localhost:3000`

## # [Mobile](https://github.com/Domeniqque/gostack-meetup-mobile)

The mobile application was available for **IOS** only and was tested on **iPhone X** simulator with IOS 12.4.

On **mobile** directory, run:

> yarn && cd ios && pod install

Before installation, run on **mobile** directory

> yarn react-native run-ios
