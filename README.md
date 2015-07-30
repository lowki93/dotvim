# Requirements

- ack

#For installation :
- git clone .... .vim
- ln -s ~/vim/vimrc ~/.vimrc
- cd vim
- git submodule init
- git submodule update

#For Mac 
to update vim on mac :
- brew install macvim --custom-icons --override-system-vim --with-lua --with-luajit

if you don't have permission to write in /usr/local
- sudo chown -R `whaomi` /usr/local

If /usr/bin is before /usr/local/bin in your $PATH, hide the system Vim so the new version is found first
- sudo mv /usr/bin/vim /usr/bin/vim72
- which vim (should return /usr/local/bin/vim)

#For linux
if you have Ubuntu 13.04 Raring Ringtail, Ubuntu 12.04 Precise Pangolin, Linux Mint 15 Olivia and Mint 13 Maya, add this repository:
- sudo add-apt-repository ppa:fcwu-tw/ppa
- sudo apt-get update

or:
install lua for linux
- sudo apt-get install lua

set symlink in /usr/local/include/

and
- cd /usr/local/src
- sudo hg clone https://code.google.com/p/vim/
- cd vim ...
- sudo ./configure --enable-multibyte --with-features=huge --disable-selinux --prefix=/usr/local --enable-luainterp=yes --with-lua-prefix=/usr
- sudo make && sudo make install
- /usr/local/bin/vim --version

if you want to use vi :
- sudo mv /usr/bin/vi /usr/bin/vi.back
-sudo mv /usr/bin/vim /usr/bin/vi
