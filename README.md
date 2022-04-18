# The EͤAͣᴛⷮ $tore
The Eat Store provides a simple way to manage apps with the Eat package manager. It's
for those who need Eat, but do not need to use a terminal.

The Eat manager is a text-only package manager, while the Eat Store is a GUI
tool for using the manager.

## Usage
To install the Eat Store, go to your terminal and run:
```shell
# ╭━━━┳━━━┳━━━━╮
# ┃╭━━┫╭━╮┃╭╮╭╮┃
# ┃╰━━┫┃ ┃┣╯┃┃╰╯
# ┃╭━━┫╰━╯┃ ┃┃ The Package Manager
# ┃╰━━┫╭━╮┃ ┃┃ for Linux
# ╰━━━┻╯ ╰╯ ╰╯
# Install python.
# Table below.
# /‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾\
# | Command                             | Distribution               |
# |-------------------------------------+----------------------------|
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

# Get PyInstaller.
python -m pip install pyinstaller

# Compile the program.
pyinstaller --name estore --windowed --onefile ./store.py

# Add to /usr/bin.
sudo install ./dist/estore /usr/bin/estore
```
Be sure to create a shortcut to `/usr/bin/estore` on your desktop.

Eat Store does not work in text-only Linux distributions. because it is written using Tkinter. 
If you need it and are using a text-only distro, you can use the text-only Eat.
