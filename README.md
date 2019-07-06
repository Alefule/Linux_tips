# Linux_tips


### Small details to customize linux

To change Dock position to top, you only need put this command in your terminal.

`gsettings set org.gnome.shell.extensions.dash-to-dock show-apps-at-top true`

### Customize terminal

To change the tipical sheel try fish:

`sudo apt-get install fish`

Use `fish` command to see the new appearance of the terminal

To access the configuration try `fish_config` and customize the parameters.

If we want to keep that shell by default we will put in the terminal `chsh -s /usr/bin/fish`

There are tools that will help us to leave the shell with a very nice appearance, `oh my fish` is a example.

To install it try `curl -L https://github.com/oh-my-fish/oh-my-fish/raw/master/bin/install | fish`

To install a new theme you need choose one: the alias `omf`, if you want the theme list put `omf list` and to install one of this try `omf install agnoster` 
Agnoster is the theme name and it's the next tip we're going to see:

If you have any problem with the fonts or you theme isn't see correctly, try to install the fonts;
`
$ sudo apt-get install python-pip
$ sudo pip install -U pip
$ sudo su
$ su -c 'pip install git+git://github.com/Lokaltog/powerline'
$ wget https://github.com/Lokaltog/powerline/raw/develop/font/PowerlineSymbols.otf https://github.com/Lokaltog/powerline/raw/develop/font/10-powerline-symbols.conf
$ sudo mv PowerlineSymbols.otf /usr/share/fonts/
$ sudo fc-cache -vf
$ sudo mv 10-powerline-symbols.conf /etc/fonts/conf.d/
$ exit
`

if everything went well you should see something like that:


