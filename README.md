# How to install virtal env for multiple Python versions
```
[root@minikube01 ~]# python3 -m pip install --user --upgrade pip
WARNING: Running pip install with root privileges is generally not a good idea. Try `__main__.py install --user` instead.
Collecting pip
  Downloading https://files.pythonhosted.org/packages/a4/6d/6463d49a933f547439d6b5b98b46af8742cc03ae83543e4d7688c2420f8b/pip-21.3.1-py3-none-any.whl (1.7MB)
    100% |████████████████████████████████| 1.7MB 684kB/s
Installing collected packages: pip
Successfully installed pip-21.3.1

```
```
python3 -m venv env
source env/bin/activate
deactivate
```
```
Installing packages
python3 -m pip install requests
```
```
Installing specific versions
python3 -m pip install requests==2.18.4
```
```
To install the latest 2.x release of requests:
python3 -m pip install requests>=2.0.0,<3.0.0
```
```
To install pre-release versions of packages, use the --pre flag:
python3 -m pip install --pre requests
```
```
Installing from source-
cd google-auth
python3 -m pip install .
```
```
Installing from local archives
python3 -m pip install requests-2.18.4.tar.gz
```
```
If you have a directory containing archives of multiple packages, you can tell pip to look for packages there and not to use the Python Package Index (PyPI) at all:
python3 -m pip install --no-index --find-links=/local/dir/ requests
```
```
If you want to download packages from a different index than the Python Package Index (PyPI), you can use the --index-url flag:
python3 -m pip install --index-url http://index.example.com/simple/ SomeProject
```
```
Upgrading packages
python3 -m pip install --upgrade requests
```
```
Installing for requirements.txt file
python3 -m pip install -r requirements.txt
```
```
Pip can export a list of all installed packages and their versions using the freeze command:
```
