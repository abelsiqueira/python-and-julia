# Docker image for Python and Julia

Docker image with Python and Julia built for interoperability.

## Scope and limitation

- Provide Julia 1.X + Python 3.Y combinations for a few values of X and Y.
- We currently use PyCall.jl and PyJulia, but that can change.

## Building

It should be automatic with every new commit, but in case you want to do it manually:

```bash
docker build -t abelsiqueira/python-and-julia:py3.10-jl1.8 \
  --build-arg PYTHON_VERSION=3.10.10 \
  --build-arg JULIA_VERSION=1.8.5
```

## License

[![Apache License](https://img.shields.io/badge/license-Apache%202.0-orange.svg?style=flat-square)](LICENSE).

### Copyright:

- 2022 Abel Soares Siqueira
- 2022 Faruk Diblen
