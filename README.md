This is a simple [Sinatra](https://www.sinatrarb.com) app that's 
deployable to [Heroku](http://heroku.com) and can act as a [logging bridge](http://help.papertrailapp.com/kb/configuration/configuring-centralized-logging-from-javascript/) for 
[Papertrail](https://papertrailapp.com). 

It uses [sinatra-cross_origin](https://github.com/britg/sinatra-cross_origin) to support CORS.

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)


Name of app in heroku => papertrail-js-logs https://dashboard.heroku.com/apps/papertrail-js-logs
The current PAPERTRAIL_API_TOKEN is set to Ruben's api token.

To connect the heroku app to our standalone papertrail account we needed to run `heroku drains:add syslog+tls://logs7.papertrailapp.com:40793`. More details on this [here](https://papertrailapp.com/systems/setup?type=app&platform=heroku)
