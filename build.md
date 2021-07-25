https://www.docker.com/blog/multi-arch-build-and-images-the-simple-way/

Version Specific
```
docker buildx build --build-arg BRANCH=v%.%.% --push --platform linux/arm64,linux/amd64 --tag lryanuk/chiadog-docker:v%.%.% .
```
Dev branch
```
docker buildx build --build-arg BRANCH=dev --push --platform linux/arm64,linux/amd64 --tag lryanuk/chiadog-docker:dev .
```
Main branch
```
docker buildx build --build-arg BRANCH=main --push --platform linux/arm64,linux/amd64 --tag lryanuk/chiadog-docker:latest .
```