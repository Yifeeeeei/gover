# gover: go version management shell function

## Install: pull and add to shell

Zsh

```shell
curl -sSL "https://raw.githubusercontent.com/Yifeeeeei/gover/main/gover" >> ~/.zshrc && source ~/.zshrc
```

If you want to reinstall, remove the gover function from ~/.zshrc manually first.

## Usage

###  List Available Versions
To see the installed Go versions available for switching:

```shell
$ gover
Usage: gover <version>
Available Go versions:
1.20.4
1.21.2
1.21.1
1.24.0

Examples:
  gover 1.20.4   # Switch to Go version 1.20.4 or download and switch
  gover 1.19     # Switch to the latest 1.19.x version available
```

### Switch to specific version

```shell
$ gover 1.24
✅ Switched to Go 1.24.3
go version go1.24.3 darwin/arm64
```

### Install and use a new go version

```shell
$ gover 1.22.0
⚠️ Go 1.22.0 is not installed. Downloading...
Downloading Go 1.22.0 for darwin-arm64...
Extracting Go 1.22.0...
✅ Go 1.22.0 installed successfully!
✅ Switched to Go 1.22.0
go version go1.22.0 darwin/arm64

```

### Automatically use the latest version

```shell
$ gover 1.24
✅ Switched to Go 1.24.3
go version go1.24.3 darwin/arm64
```

## Uninstall

Go to ~/.zshrc and delete the function gover.
