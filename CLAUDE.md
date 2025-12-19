# Koffan - Rules for Claude

## Docker Image

After every push to origin public (PanSalut/Koffan), build and push a new Docker image:

```bash
docker build -t ghcr.io/pansalut/koffan:latest .
docker push ghcr.io/pansalut/koffan:latest
```

Requires prior login:
```bash
gh auth token | docker login ghcr.io -u PanSalut --password-stdin
```
