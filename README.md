# The ɐǝt $tore
The Eat Store provides a simple way to manage apps with the Eat package manager. It's
for those who need Eat, but do not need to use a terminal.

The Eat manager is a text-only package manager, while the Eat Store is a GUI
tool for using the manager.

## Install
### Manual
To install the Eat Store, go to your terminal and run:
```shell
# ╭━━━┳━━━┳━━━━╮
# ┃╭━━┫╭━╮┃╭╮╭╮┃
# ┃╰━━┫┃ ┃┣╯┃┃╰╯
# ┃╭━━┫╰━╯┃ ┃┃ The Package Manager
# ┃╰━━┫╭━╮┃ ┃┃ for 𝕃𝕚𝕟𝕦𝕩
# ╰━━━┻╯ ╰╯ ╰╯
# Install python.
# Table below.
# /******************************************************************\
# | Command                             | Distribution               |
# | ------------------------------------+--------------------------- |
# | sudo apt install python3            | Ubuntu                     |
# | sudo apt install python-is-python3  |                            |
# | ------------------------------------+--------------------------- |
# | sudo pacman -S python               | Arch                       |
# | ------------------------------------+--------------------------- |
# | pkg install python                  | Android (Termux)           |
# | ------------------------------------+--------------------------- |
# | eatinst python                      | Any distro (user only)     |
# \__________________________________________________________________/
# Ensure you have Python 3 by running: python -V

# Clone and change working directory.
git clone https://github.com/EatInstall/Store.git
cd Store

# Get PyInstaller.
python -m pip install pyinstaller

# Compile the program.
pyinstaller --name estore --windowed --onefile ./store.py

# Add to /usr/bin.
sudo install ./dist/estore /usr/bin/estore
```
Be sure to create a shortcut to `/usr/bin/estore` on your desktop.

Eat Store does not work in text-only Linux distributions (e.g. Ubuntu Server), because it is written using Tkinter. 
If you need it and are using a text-only distro, you can use the text-only Eat.

Using the `git` protocol will not work, you'll get an error.
### Debian PacKaGe (`dpkg`) tool
If you are a Ubuntu or Debian user, you can build and install the Debian package `eat-store.deb`:
```shell
git clone https://github.com/EatInstall/Store.git
cd Store
dpkg-buildpackage
sudo dpkg -i eat-store.deb
# idealy; you can also choose apt (sudo apt install --yes ./eat-store.deb)
```
