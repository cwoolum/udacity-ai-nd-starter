# Udacity AI Nanodegree development environment

I built this small starter for the Udacity AI nanodegree program. Rather than installing Python on your machine, if you have Docker installer, you can just clone this repo, open it in VS Code and it will automatically install everything that you need to run a full Python environment in a container, keeping your host system clean.

> See more info [here](https://code.visualstudio.com/docs/remote/containers#_quick-start-try-a-dev-container) on using Dev Containers.

This project does require the `ms-vscode-remote.remote-containers` extension to work.

After opening this in VS Code, You can clone the projects repository into the root of this folder to work on your projects.

## Working on the Pacman project

Because this is operating in a container, you'll need to do a but of extra configuration.

1. Install [XcXsrv](https://sourceforge.net/projects/vcxsrv/)

2. Make sure that XcXsrv is running

3. Get the ip address for the host machine. Open a command prompt and run `ipconfig | findstr /C:Address`. You want the `IPv4 Address`. If there are multiple, it's most likely the one that starts with `192.168.`. Run the command `export DISPLAY=IP_ADDRESS:0.0` where `IP_ADDRESS` is the one you got from the previous command.

You should now be able to run all of the Pacman simulations!
