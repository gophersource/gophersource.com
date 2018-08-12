---
title: Setup
description: Get ready to write Go!
menu: main
---

Before you can contribute to Go projects, you will need a working developer
environment.

1. **Install Go**<br/>
    Follow the instructions for your operating system to install Go:

    * [Mac](https://golang.org/doc/install#osx)
    * [Windows](https://golang.org/doc/install#windows)
    * [Ubuntu](https://github.com/golang/go/wiki/Ubuntu)

1. **Understand your GOPATH**<br/>
    The GOPATH is the location where Go looks for source code, caches packages, etc.
    You do not need to set it explicitly and can run the following comment to see where
    Go thinks your GOPATH is.

    ```
    $ go env GOPATH
    /Users/carolynvs/go
    ```

    By default your GOPATH is in your home directory, ~/go.
    You can change it by setting the GOPATH environment variable.

1. **Add GOPATH/bin to your PATH**<br/>
    When you install a Go application, it is placed under GOPATH/bin. You should
    add that location to your PATH environment variable. This allows you to easily
    install and run apps.

    On Mac and Linux, modify your shell profile, such as ~/.bashrc, ~/.bash_profile or ~/.profile, and add the following line:

    ```
    export PATH=$PATH:$(go env GOPATH)/bin
    ```

    On Windows, run the following powershell command to permanently modify your
    PATH environment variable:

    ```
    [System.Environment]::SetEnvironmentVariable('PATH', $env:Path + ";$(go env GOPATH)\bin", [System.EnvironmentVariableTarget]::User)
    ```

1. **Verify your setup**<br/>
    Let's verify that Go is setup properly by installing a running a go application.

    ```
    $ go get -u github.com/carolynvs/magic
    $ magic
  🎵  Oh oh it's magic! 🎵
    ```

<center>
  <img alt="gophers at work" src="/img/build.png" width="256"/>
</center>
