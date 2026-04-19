Sample Python
-------------

Setup Local Python Environment:

(If the Python install fails, see: https://github.com/pyenv/pyenv/wiki/Common-build-problems)

Run the server locally:
```
python main.py
```

Check it out: http://localhost:8080

Run Locally with Buildpacks & Docker:
```
pack build --builder=gcr.io/buildpacks/builder sample-python
docker run -it -ePORT=8080 -p8080:8080 sample-python
```

Run on Cloud Run:

[![Run on Google Cloud](https://deploy.cloud.run/button.svg)](https://deploy.cloud.run)
