---
title: Setup
description: Get ready to write Go!
image: "/img/build.png"
---

1. **Install Go**

    **MacOS**

    Download the [Go installer](https://golang.org/dl/) for macOS and run it.

    **Windows**

    Download the [Go installer](https://golang.org/dl/) for Windows and run it.

    **Ubuntu**
    
    ```
    curl -sLO https://godeb.s3.amazonaws.com/godeb-amd64.tar.gz
    tar -xzf godeb-amd64.tar.gz
    ./godeb install
    ```

1. **Understand your GOPATH**

    The GOPATH is the location where Go looks for source code, caches packages, etc.
    You do not need to set it explicitly and can run the following comment to see where
    Go thinks your GOPATH is.

    ```console
    $ go env GOPATH
    /Users/carolynvs/go
    ```

    By default your GOPATH is in your home directory, ~/go.
    You can change it by setting the GOPATH environment variable.

    Go requires that a project's source code is located in **GOPATH/src/PACKAGE_NAME**,
    for example GOPATH/src/github.com/carolynvs/magic or GOPATH/src/golang.org/x/golint.

1. **Add GOPATH/bin to your PATH**

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

    After you have update your PATH environment variable, open a new shell window or tab
    so that it is loaded and ready for you to use.

1. **Verify your setup**

    Let's verify that Go is setup properly by installing a running a go application.

    ```console
    $ go get -u github.com/carolynvs/magic
    # the source is downloaded to GOPATH/src/github.com/carolynvs/magic

    $ magic
  🎵  Oh oh it's magic! 🎵
    ```

    The `go get -u` command clones the package's source code under the GOPATH in
    its proper place, or updates it if it already exists, builds the package
    and then installs it. Because we put GOPATH/bin on our PATH, the binary built
    by Go, `magic`, is available for us to use immediately.


<center>
  <img alt="gophers at work" src="/img/build.png" width="256"/>
</center>
