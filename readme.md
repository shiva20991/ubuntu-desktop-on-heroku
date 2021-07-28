# Ubuntu Desktop on Heroku

A [Heroku](https://www.heroku.com/) install of [Ubuntu 20.10 (Groovy Gorilla)](https://releases.ubuntu.com/20.10/), with the [XFCE desktop environment](https://www.xfce.org/) and [VNC](https://en.wikipedia.org/wiki/Virtual_Network_Computing).

Do an automated deploy to Heroku:
href="https://heroku.com/deploy?template=https://github.com/shiva20991/ubuntu-desktop-on-heroku">
  <img src="https://www.herokucdn.com/deploy/button.svg" alt="Deploy">
</a>
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Built With

- [noVNC](https://novnc.com/)

## Run Locally

Install [Docker](https://docs.docker.com).

Build and run the container with Docker.

## Deploy to Heroku

Install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli).

Create a Heroku app:
```bash
heroku create
```

Note the Heroku app name, and add the Heroku Git repository as a remote to this Git repository:
```bash
heroku git:remote -a [heroku-app-name]
```

Set the app's stack to container:
```bash
heroku stack:set container -a [heroku-app-name]
```

Deploy the app:
```bash
git push heroku master
```

Now open the app in your browser:
```bash
heroku open
```
