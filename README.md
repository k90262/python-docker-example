## Simple python docker dev example for the official docker docs
https://docs.docker.com/language/python/containerize/


----
## Run program with required module (Not use docker) 

> (Using `venv` to install dependent packages on a local folder we assigned)

Demo Steps:
```shell
git clone https://github.com/k90262/python-docker-example.git
cd python-docker-example
# python3 app.py # Throw Error! it cannot import FastAPI module
python3 -m venv .venv
source .venv/bin/activate
> pip install -r requirements.txt
> pip install uvicorn
> uvicorn app:app --reload
deactivate
```