# Data analysis
- Document here the project: bbquote
- Description: Project Description
- Data Source:
- Type of analysis:

Please document the project the better you can.

# Startup the project

The initial setup.

Create virtualenv and install the project:
```bash
  $ sudo apt-get install virtualenv python-pip python-dev
  $ deactivate; virtualenv ~/venv ; source ~/venv/bin/activate ;\
    pip install pip -U; pip install -r requirements.txt
```

Unittest test:
```bash
  $ make clean install test
```

Check for bbquote in gitlab.com/{group}.
If your project is not set please add it:

- Create a new project on `gitlab.com/{group}/bbquote`
- Then populate it:

```bash
  $ ##   e.g. if group is "{group}" and project_name is "bbquote"
  $ git remote add origin git@gitlab.com:{group}/bbquote.git
  $ git push -u origin master
  $ git push -u origin --tags
```

Functionnal test with a script:
```bash
  $ cd /tmp
  $ bbquote-run
```
# Install
Go to `gitlab.com/{group}/bbquote` to see the project, manage issues,
setup you ssh public key, ...

Create a python3 virtualenv and activate it:
```bash
  $ sudo apt-get install virtualenv python-pip python-dev
  $ deactivate; virtualenv -ppython3 ~/venv ; source ~/venv/bin/activate
```

Clone the project and install it:
```bash
  $ git clone gitlab.com/{group}/bbquote
  $ cd bbquote
  $ pip install -r requirements.txt
  $ make clean install test                # install and test
```
Functionnal test with a script:
```bash
  $ cd /tmp
  $ bbquote-run
```