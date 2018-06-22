# Motivational Penguin

**This Messenger bot was created at the Wetton Workshop 2018 Hack Day by Mike Walmsley.**

Talk to me [here](https://www.facebook.com/Motivational-Penguin-383781245444076/). I can tell you sentences about the astronomer Argelandar.

I'm running on a node.js server (mostly boilerplate from Facebook), within a docker container, hosted on Heroku. I communicate with Facebook via webhooks.

/app contains the node.js server and associated Dockerfile.

Send me to Heroku with the following commands:

1. `cd app` (from penguin root)
2. Build and push Dockerfile to Heroku app motivational-penguin app as a web dyno: `heroku container:push web --app motivational-penguin`
3. Update the current web dyno with the new image: `heroku container:release web --app motivational-penguin`

You will need the Heroku CLI installed, and the app motivational-penguin created.

To run locally, use localtunnel to turn the local server port into a web address that Facebook can communicate with. Warning: localtunnel can be flaky.

1. `docker-compose build` (from penguin root)
2. `docker-compose up`

This launches a container for app (the node.js server) linked to a second container running localtunnel. **Warning: I haven't quite got the localtunnel launch command right, so this is currently broken.**

*Because I'm a bot, not a website, it's not easy to check I'm working okay. Navigate to [my url]/check to see if I'm definitely alive - you should recieve a status 200 'OK' response if so.*

#### Further information from Facebook

This is a sample project showcasing the Messenger Platform. You can go through the [walk-through](https://developers.facebook.com/docs/messenger-platform/guides/quick-start) to understand this code in more detail. The [Complete Guide](https://developers.facebook.com/docs/messenger-platform/implementation) goes deeper into the features available.

Visit the [dev site](https://developers.facebook.com/docs/messenger-platform/) to find out more details about the Messenger Platform.

