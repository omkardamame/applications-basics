
## Install python (CentOS/ RHEL)

```bash
yum install python2
```

This one below will install Python 3.6,

```bash
yum install python36
```

## To invoke the interpreter,

For Python2

```bash
python2
```

For Python3.6

```bash
python3
```

## To see the versions of them

```
python2 -V
```

```
python3 -V
```

## To run python program,

```bash
python3 test.py
```

## Python Package Manager (pip)

These are the commands to see versions,

![[python_version.png]]

## Python file system

![[python_file_system.png]]

To install a package, this is an example command,

```bash
pip install flask
```

This command shows package metadata,

```bash
pip show flask
```

![[python_pip.png]]

## Requirements file

An application may have multiple dependencies and those dependencies might break with upgrades of their versions. Rather than installing those dependencies multiple times with possibility of  losing backwards compatibility too, you can create a requirements file in which all the necessary dependencies along with their versions are listed. This file can install all the dependencies at once.

```bash
pip install -r requirements.txt
```

Example requirements.txt
```
Flask==0.10.1

Jinja==2.7.3

MarkupSafe==0.23

and so on..
```

## Upgrade/Uninstall pip packages

Upgrade a package,

```bash
pip install flask --upgrade
```

Uninstall a package,

```bash
pip uninstall flask
```

