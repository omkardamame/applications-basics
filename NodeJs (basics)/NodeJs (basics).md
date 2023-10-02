
## Installation (CentOS 7)

```bash
curl -sL https://rpm.nodesource.com/setup_14.x | sudo bash -;sudo yum install -y nodejs
```

## Check version

```bash
npm -v
```

**NPM**: Node Package Manager
Used for reusing package modules and to share.

`npsjs.com` hosts public repository for the modules.

## Install package

NPM search will search the package if installed or not and it's dependencies. Also, it will list all packages available by that name and its information.

```bash
npm search file
```

```bash
npm install file
```

When you install a package, NPM installs it under the directory `node_modules`. The code for it is located in `lib` directory. We have installed package in current directory/project only. We haven't installed for for global usage.

To install node package globally use following command,

```bash
npm install file -g
```

![[nodejs_pkg.png]]

Also, there is a file called `package.json` which contains metadata for that package. This is a useful file for troubleshooting issues with dependency errors.

![[nodejs_package_json.png]]

## Command modules

Only built-in modules are installed along with NPM.

![[nodejs_modules.png]]

Built-In modules path,

```
/usr/lib/node_modules/npm/node_modules
```

External modules path

```
/usr/lib/node_modules
```

## Application dependencies

`package.json` file consist of dependencies required for the application.

![[nodejs_dependencies.png]]