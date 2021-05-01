# Heroku

## Container
```
heroku config:set POD_TOKEN=joesmith -a bot-recorder
heroku config:set POD_ROLES=admin -a bot-recorder
heroku config:set POD_OUTPUT_FORMAT=mp3 -a bot-recorder
heroku config:set POD_PREFIX=* -a bot-recorder

heroku stack:set container -a bot-recorder
```

## Scaling
```
heroku ps:scale web=0 -a bot-recorder
```
## Debug
```
heroku run bash -a bot-recorder
```
## Plugins
```
heroku plugins:install heroku-builds
heroku builds -a bot-recorder
heroku builds:cancel -a YOUR_HEROKU_APP_NAME
```
