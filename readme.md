## commands

```bash
docker run -it --rm -v "$PWD:/code" node:14-alpine sh -c 'node -v; npm -v; npm install --prefix=/code'
```

```bash
docker run -it --rm -v "$PWD:/code" node:12-alpine sh -c 'node -v; npm -v; npm install --prefix=/code'
```

```bash
docker run -it --rm -v "$PWD:/code" node:16-alpine sh -c 'node -v; npm -v; npm install --prefix=/code'
```
