# Requirements

- ag
- js (or any js interpreter, for jslint)
- exuberant ctags
- a solarized terminal
- powerline fonts
- ack

#For installation :
- git clone .... .vim
- ln -s ~/vim/vimrc ~/.vimrc
- cd vim
- git submodule init
- git submodule update

to update vim on mac : 
- brew install macvim --custom-icons --override-system-vim --with-lua --with-luajit

if you don't have permission to write in /usr/local
- sudo chown -R `whaomi` /usr/local

If /usr/bin is before /usr/local/bin in your $PATH, hide the system Vim so the new version is found first
- sudo mv /usr/bin/vim /usr/bin/vim72
- which vim (should return /usr/local/bin/vim)
