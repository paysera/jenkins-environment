# jenkins-environment
### Initial setup
##### Copy data into storage's
```bash
docker cp data/ssh jenkinsenvironment_jenkins_1:/var/jenkins_home/.ssh
docker exec -it -u root jenkinsenvironment_jenkins_1 sh -c 'chown -R jenkins:jenkins /var/jenkins_home/.ssh'
```

### Control
##### Start/restart environment
```bash
./scripts/launch.sh
```