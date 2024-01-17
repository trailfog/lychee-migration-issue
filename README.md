# Minimal repo for reproducing upgrade issue of lychee `5.0.2` -> `5.0.3`

1. Run `docker compose up -d`
2. Head over to [http://localhost:8080](http://localhost:8080) and set up the instance with an admin account
3. Change the docker image of `lychee` to `lycheeorg/lychee:v5.0.3`
4. Run `docker compose up -d`
5. Reload the page [http://localhost:8080](http://localhost:8080) and be greeted with a login
6. After the login, you can see the Migration result of `Branch is not master`

If the image is downgraded back to `v5.0.2`, everything works as expected.
