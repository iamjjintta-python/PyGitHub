# PyGitHub
Simple GitHub API with Python

## Install
```sh
$ pip install iamjjintta-pygithub
```

## Example
```python
from iamjjinta.github import GitHub


username = 'Your GitHub Username'
password = 'Your GitHub Password'

# GitHub Login
github = GitHub(username, password)
login = github.login()
print(login.status_code)

# Get Repository Content
owner = 'iamjjintta-python'
repo = 'PyGitHub'
branch = 'main'
path = '/iamjjintta/github.py'

source_code = github.get_content(owner, repo, branch, path)
print(source_code)
```
