# lock-wtf

> `lockfileVersion` hell :fire: :fire_extinguisher:

## commands

### node 14.x; npm 6.x

```bash
docker run -it --rm -v "$PWD:/code" node:14-alpine sh -c 'node -v; npm -v; npm install --prefix=/code'

git diff package-lock.json
# no changes
```

### node 16.x; npm 8.x

```bash
docker run -it --rm -v "$PWD:/code" node:16-alpine sh -c 'node -v; npm -v; npm install --prefix=/code'

git diff package-lock.json
# +  "lockfileVersion": 2,
# -  "lockfileVersion": 1,
```

### node 14.x; npm 8.x

```bash
docker run -it --rm -v "$PWD:/code" node:14-alpine sh -c 'node -v; npm -v; npm i -g npm@latest; npm -v; npm install --prefix=/code'

git diff package-lock.json
# +  "lockfileVersion": 2,
# -  "lockfileVersion": 1,
```
