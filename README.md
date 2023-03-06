# Requirements
1. This was tested with Docker version `23.0.1` and docker-compose version `1.25.0`.
2. Authorize in Github using this [tutorial](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry#authenticating-with-a-personal-access-token-classic):

  a. Create a Personal Access Token (PAT).

  b. `export CR_PAT=YOUR_TOKEN`

  c. `echo $CR_PAT | docker login ghcr.io -u USERNAME --password-stdin`

3. The `.env` file is expected in the same directory as `docker-compose.yaml`
# Run
In terminal:
```
docker-compose up
```

# Access GUI/Swagger
Visit `127.0.0.0/docs` in browser.

# Available Services
- `API`: port 80
- `redis`: port 6379
- `rabbitmq`: port 5672
