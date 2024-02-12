# Build image
```
# run from root of repo for raspi
docker image build --platform linux/arm64 -t stvoffutt/flask-hello-world:arm64 -f flask-hello-world/Dockerfile flask-hello-world
```