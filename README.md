# swarm-stack-core
Core containers for running on swarm

## Environment Vars

Create an `env` file with these in there:

```
export LOGSPOUT_NAME="swarm"
export LOGSPOUT_COMMAND="syslog://logs5.papertrailapp.com:9999"
export TRAEFIK_LOG=WARN
export DOMAIN="swarm.com"
export LETSENCRYPT_EMAIL="swarm@example.com"
export DEPLOY_SLACK_HOOK="https://hooks.slack.com/services/xxx"
export DEPLOY_SECRET="changeme"
export GITHUB_USERS=user1
```

## Usage

```
source env && docker stack deploy -c core.yml core
```

