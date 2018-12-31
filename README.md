# Seki Server

## Run

1. Run `ngrok 8080`
2. Create an OAuth Application as showed in [drone docs](https://docs.drone.io/intro/bitbucket-cloud/single-machine/). Put ngrok url as callback.
3. Create `drone_config.env`
```
DRONE_USER_FILTER=<bitbucket_user>
DRONE_BITBUCKET_CLIENT_ID=<consumer_key>
DRONE_BITBUCKET_CLIENT_SECRET=<consumer_secret>
DRONE_SERVER_HOST=<ngrok_url>
```
4. Run docker
```
docker-compose up
```
5. Enjoy!
