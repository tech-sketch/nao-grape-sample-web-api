# google_stt

Google speech to text sample

## Environment
* Python 2.7 or 3.5

## Install

```bash
$ cd /path/to/google_stt
$ virtualenv .venv
$ source .venv/bin/activate
(.venv)$ pip install -r requirements.txt
```

## Setting API KEY

Check your key from https://console.developers.google.com

```python
# apikey = os.environ.get("GOOGLE_API_KEY")
apikey = "YOUT_API_KEY_HERE"
```

Or if you use [autoenv](https://github.com/kennethreitz/autoenv),

```bash
$ cp .env.sample .env
$ vi .env  # update your api key
$ cd ..
$ cd google_stt  # apply api key as a environment variable
```

Or if you use [direnv](https://github.com/direnv/direnv),

```bash
$ cp .env.sample .envrc
$ vi .envrc  # update your api key
$ cd ..
$ cd google_stt  # apply api key as a environment variable
```

## Usage

```bash
$ python stt.py test.wav "ja-JP"
白石です
```
