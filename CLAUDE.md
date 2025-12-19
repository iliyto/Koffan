# Koffan - Zasady dla Claude

## Docker Image

Po każdym pushu na origin public (PanSalut/Koffan), zbuduj i wypchnij nowy obraz Docker:

```bash
docker build -t ghcr.io/pansalut/koffan:latest .
docker push ghcr.io/pansalut/koffan:latest
```

Wymaga wcześniejszego zalogowania:
```bash
gh auth token | docker login ghcr.io -u PanSalut --password-stdin
```
