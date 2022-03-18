# MacOS

## 1. Install homebrew
Homebrew is a widely used package manager for MacOS. It provides clean, convenient access to a variety of command line tools as well as making them easy to maintain and upgrade as updates are released.

1. Launch your `Terminal`.
2. Follow the installation instructions at [brew.sh](https://brew.sh/).

    **NOTE:** `brew` is widely used, recognized, and trusted (although it certainly has security tradeoffs). However, **always** think twice before running scripts, commands, or software that you aren't familiar with! If you aren't sure if something is safe to run or install, please reach out to a teammate.
3. Run `brew --version`.
    Confirm that you see something like the following:
    ```
    Homebrew 3.3.16
    Homebrew/homebrew-core (git revision abd084f128d; last commit 2022-02-22)
    ```

If they weren't already installed, the install script should install the MacOS [Command Line Tools](https://developer.apple.com/xcode/features/) as well.

## 2. Install a version manager
When you start development on a brand new application, you can (and usually should!) choose to use the latest stable version of whatever tools you'll be using to build it. However, as software developers, we often work with older code and code written by (sometimes many) other people.

This can mean switching between many different versions of the same library. Installing and swapping between these versions can become tedious and, worse, project environments may collide with each other or not work as expected.

This is exactly why version managers exist! A version manager allows us to have multiple installs of different versions of the same tool, language, or framework co-existing in perfect harmony. As the name suggests, it _manages versions_ (most commonly of programming languages).

1. Determine your current shell
    Some versions of MacOS come with a different default shell. To determine your shell, run `echo $SHELL` in your terminal.

    It should return something like `/bin/{YOUR SHELL}` and the value of `{YOUR SHELL}` should be one of `zsh` or `bash`.
2. Follow the `asdf` install instructions for "`{YOUR SHELL}` and Homebrew" [here](https://asdf-vm.com/guide/getting-started.html). 

### 2a. Install frameworks
From here on out, when you have to install a programming language, you can install it via `asdf`.

**To add the plugin for a specificl tool**

`asdf plugin add {NAME} {GIT URL}`
- `{NAME}`: name of the plugin (e.g., `ruby` for the Ruby version management plugin)
- `{GIT URL}`: URL for the git repository of the plugin (e.g., `https://github.com/asdf-vm/asdf-ruby` for `asdf-ruby`)

**To install the latest version**

`asdf install {NAME} latest`
- `{NAME}`: name of the plugin (e.g., `ruby` for the Ruby version management plugin)

**List all available versions**

`asdf list all {NAME}`
- `{NAME}`: name of the plugin (e.g., `ruby` for the Ruby version management plugin)

**To install a specific version**

`asdf install {NAME} {VERSION}`
- `{NAME}`: name of the plugin (e.g., `ruby` for the Ruby version management plugin)
- `{VERSION}`: the specific version you want to install


If you need to perform any other operations, please refer to [the `asdf` documentation](https://asdf-vm.com/manage/core.html) as well.


**NOTE:** This guide recommends `asdf`, but there are [many awesome version managers](https://github.com/bernardoduarte/awesome-version-managers) available.
