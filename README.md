# gitlab-runner-compose
Docker compose for gitlab runner

## update the config/gitlab-runner/config.toml
- change the GITLAB_RUNNER_TOKEN to your token base on repository of gitlab under CI/CD
- if you're testing other images change the node:12-alpine to desired image

## running the runner
```
docker-compose up -d
docker-compose run gitlab-runner bash
```

You're now inside the container
```
gitlab-runner register # if you want to update the config
gitlab-runner verify # to update the status to gitlab
```
