# Install Emscripten Package

## Usage

### Default Version Numbers

```yml
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: HandcrankEngine/install-emscripten-package@v0.2.0
```

### Specific Version Numbers

```yml
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: HandcrankEngine/install-emscripten-packages@v0.2.0
        with:
          EMSDK_VERSION: "6.0.7"
          CACHE_EMSCRIPTEN: "true"
```

## Inputs

| Name               | Description                                      | Default |
| :----------------- | :----------------------------------------------- | :-----: |
| `EMSDK_VERSION`    | Emscripten version                               | `6.0.7` |
| `CACHE_EMSCRIPTEN` | If the action should cache the Emscripten files. | `true`  |
