# Popup Vue Development Tool
> A Todd Project

- [Installation](#installation)
  * [Installation Flags](#installation-flags)
- [Development](#development)

# <a name="installation"></a> Installation
An installation script is provided to streamline the install. 
If this is a fresh install just run `./install` and you're good
to go. 

This will load the required dependencies and create the settings file.
It will also remove the .git directory. Removing the application from
git will allow a new repo to be created. 

## <a name="installation-flags"></a> Installation Flags

Run `./install -h` for usage:
```
Usage: no parameters attempts to perform a fresh install
       [-r] reinstall application.
       [-n] re/install dependencies.
       [-s] install/reset settings.
       [-h] show usage.
```

# <a name="development"></a>Development 

`yarn run dev` serve with hot reload at localhost:8080


`yarn run build` build for production with minification 

