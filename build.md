https://www.docker.com/blog/multi-arch-build-and-images-the-simple-way/

Version Specific
```
docker buildx build --push --platform linux/arm64,linux/amd64 --tag lryanuk/chiadog-docker:v%.%.% .
```
Latest
```
docker buildx build --push --platform linux/arm64,linux/amd64 --tag lryanuk/chiadog-docker:latest .
```