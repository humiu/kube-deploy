# [humiu/kube-deploy](https://hub.docker.com/r/humiu/kube-deploy) - Alpine docker image with kubectl and envsubst

Alpine docker image with kubectl and envsubst for automated multi-stage Kubernetes deployments (e.g. for use in CD pipelines).

The [envsubst](https://www.gnu.org/software/gettext/manual/html_node/envsubst-Invocation.html) command can be used to [inject environment variables](https://stackoverflow.com/a/56009991/2524925) into kubernetes resource files.

### Build the docker image

```bash
DOCKER_USER_NAME=<your docker username>
docker build -t $DOCKER_USER_NAME/kube-deploy .
```

### Test the docker image

```bash
docker run -ti --rm $DOCKER_USER_NAME/kube-deploy
```

### Push the kube-deploy image to docker hub

```bash
docker push $DOCKER_USER_NAME/kube-deploy
```
