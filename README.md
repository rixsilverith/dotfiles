<h1 align="center">Dotfiles and Configs</h1>
<p align="center">
<img style="margin:5px;" src="https://img.shields.io/github/license/rixsilverith/dotfiles?style=flat-square"/>
<img style="margin:5px; "src="https://img.shields.io/badge/distro-Arch-48b9c7?style=flat-square"/>
<img style="margin:5px; "src="https://img.shields.io/badge/wm-bspwm-48b9c7?style=flat-square"/>
</p>

<p align="center">
  <img src=".github/desktop.png" width="85%">
</p>

<p align="center">
  <a href="#-installation">Installation</a>&nbsp;&nbsp;•&nbsp;
  <a href="bin/dot"><code>dot</code></a>&nbsp;&nbsp;•&nbsp;
  <a href="scripts">Scripts</a>&nbsp;&nbsp;•&nbsp;
  <a href="git/.gitconfig">Git configuration</a>
</p>

## Installation
The installation of this dotfiles is pretty straightforward: just run the next command in your terminal and follow the installation process.
```bash
bash <curl -s https://raw.githubusercontent.com/rixsilverith/dotfiles/master/installer>
```

## Running the `dot` command
The `dot` command is key here, as it is the main utility you'll use to manage this dotfiles, and it acts as the entry point for most of the scripts available. Once the dotfiles are installed in your system you should be able to execute `dot` in your terminal of choice to get a full list of the available scripts. The syntax is as follows:
```bash
dot <context> [subcontext] <cmd> [<args>...]
```
In a few words, a *context* is a group of related scripts. For instance, the scripts under the `net` context do stuff with network connections and interfaces, and so on.

## Updating the dotfiles
Updating the dotfiles is as simple as running `dot self update` in your terminal. This script will check for updates by looking the [dot](bin/dot) file in this repo and comparing it with the one you have in your machine. If an updated version is found, the `update` script will ask you if you wanna procceed with the installation. You can check the current version by running `dot -v`.

*Warning*: Note that this process may break your system configuration, and for this reason is strongly recommended to backup your current dotfiles folder before installing the update, by default `$HOME/.dotfiles`.

## References
- The `dot` command, as well as some scripts in these dotfiles, is pretty much based on the [denisidoro](https://github.com/denisidoro/dotfiles) and [rgomezcasas](https://github.com/rgomezcasas/dotfiles) developed for their own dotfiles.

- The custom GTK theme and icons are the work of [Juicyexe](https://github.com/Juicyexe/arch-monochrome).

## License
The MIT License. See [License](LICENSE) for more information.
