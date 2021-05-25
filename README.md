# Rails Boilerplate for Goldbelly Code Test

This is a standard Rails project starting point. We're using:

- ruby @ 2.5.9
- Rails @ 6.1.3
- rspec @ 5.0.0

It's not required to use rspec for your tests, but it's common so we've included it here.

Below are instructions for getting up and running.

## Docker

```bash
docker compose build
docker compose up -d
docker compose run web rails db:create
```

You should now be able to access the running app in your browser from http://localhost:3000

If port 3000 is already taken you can edit the docker-compose.yml file and change `"3000:3000"` to `"4321:3000"` where "4321" is your desired port.

### Clean up

When you're done working locally you can stop the containers and remove the image you built so you can regain some hard drive space :)

```bash
docker compose down
docker rmi goldbelly-code-test-rails-boilerplate_web
```

