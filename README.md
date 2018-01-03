# jenkins-pipeline-scm

### Need Docker socket inside of Jenkins to allow Jenkins to use Docker:

```
> docker run -v /var/run/docker.sock:/var/run/docker.sock -v ~/data/jenkins_docker_home:/var/jenkins_home -d --name jenkins -p 8080:8080 jenkins:latest

Has problems with 'docker' runtime missing.
```

```
Used Bitnami's Jenkins VM image with VirtualBox.  Much better.
```
> sudo chmod ogu+rwx /var/run/docker.sock
```
