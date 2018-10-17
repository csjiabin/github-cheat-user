# github-cheat-user

A blacklist program that collects cheating users on GitHub。

## Usage

```bash
git clone https://github.com/csjiabin/github-cheat-user.git
cd github-cheat-user
virtualenv -p python3 venv
source venv/bin/activate
pip install -r requirements.txt

python hub.py -h
# usage: hub.py [-h] [-t USER] [-r REPO] [-k TOKEN] [-x] [-v]

# optional arguments:
#   -h, --help            show this help message and exit
#   -t USER, --track USER
#                         track cheat users from USER
#   -r REPO, --repo REPO  track cheat users from REPO
#   -k TOKEN, --token TOKEN
#                         GitHub TOKEN
#   -x, --recheck         recheck log.md
#   -v, --version         show version
```

**Track User**

```bash
python hub.py -k YOUR_GITHUB_TOKEN -t ReenStick
```

**Recheck**

```bash
python hub.py -k YOUR_GITHUB_TOKEN -x
```
