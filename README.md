# My OSX Configuration

## Applications to download

+ [**Googe Chrome**](https://github.com/shouston3/My-Config/tree/master#googe-chrome) - My browser choice

+ [**Karabiner-Elements**](https://github.com/shouston3/My-Config/tree/master#karabiner-elements) - For key remappings

+ [**Spectacle**](https://github.com/shouston3/My-Config/tree/master#spectacle) - For quick setting of application window sizes

+ [**Iterm2**](https://github.com/shouston3/My-Config/tree/master#iterm2) - For a better terminal

## Programs to install

+ [**Zsh**](https://github.com/shouston3/My-Config/tree/master#zsh)

+ [**Vim**](https://github.com/shouston3/My-Config/tree/master#vim)

+ [**Homebrew**](https://github.com/shouston3/My-Config/tree/master#homebrew)

+ [**Git**](https://github.com/shouston3/My-Config/tree/master#git)

+ [**Sass**](https://github.com/shouston3/My-Config/tree/master#sass)

+ [**Node**](https://github.com/shouston3/My-Config/tree/master#node)

+ [**Elixir**](https://github.com/shouston3/My-Config/tree/master#elixir)

+ [**Python**](https://github.com/shouston3/My-Config/tree/master#python)

+ [**Postgres**](https://github.com/shouston3/My-Config/tree/master#postgres)

+ [**Redis**](https://github.com/shouston3/My-Config/tree/master#redis)

+ [**Heroku toolbelt**](https://github.com/shouston3/My-Config/tree/master#heroku-toolbelt)

+ [**Grip**](https://github.com/shouston3/My-Config/tree/master#grip)

## Misc

+ [**Misc**](https://github.com/shouston3/My-Config/tree/master#misc-1)
+ [**Config installation**](https://github.com/shouston3/My-Config/tree/master#config-installation)

----

#### Googe Chrome

**`Settings > Preferences > Theme > Dark`**

**Extensions**:

<img src="https://raw.githubusercontent.com/philc/vimium/master/icons/icon128.png" align="right" height="80" />

+ [Vimium](https://chrome.google.com/webstore/detail/vimium/dbepggeogbaibhgnhhndojpepiihcmeb?hl=en) - Allows for browsing the web without leaving your keyboard

<br><br>

<img src="http://core0.staticworld.net/images/article/2013/03/splash-100030679-large.jpg" align="right" height="80" />

+ [Lastpass](https://www.lastpass.com/) - For managing all your passwords

<br><br>

<img src="http://www.yournerdybestfriend.com/wp-content/uploads/2013/07/color-picker-icon_final.jpg" align="right" height="80" />

+ [Colorzilla](http://www.colorzilla.com/) - For picking colours from your browser

<br><br>

<img src="https://getadblock.com/images/adblock_logo_stripe_test.png" align="right" height="80" />

+ [Adblock](https://chrome.google.com/webstore/detail/adblock/gighmmpiobklfepjocnamgkkbiglidom) - Because I don't like seeing adverts

<br><br>

<img src="https://github.com/maximelebreton/quick-javascript-switcher/raw/master/src/icons/icon-48.png" align="right" height="80" />

+ [Quick Javascript Switcher](https://chrome.google.com/webstore/detail/quick-javascript-switcher/geddoclleiomckbhadiaipdggiiccfje) - I like to turn this off and on

<br><br>

----

#### Karabiner-Elements

<img src="https://dl2.macupdate.com/images/icons256/25141.png" align="right" height="150px" />

The only feature I use is remapping my `Caps-Lock` key to `Esc` when tapped and to `Ctrl` when held

This can be set up by importing the `Change caps_lock key` modifier keys sample from [pqrs](https://pqrs.org/osx/karabiner/complex_modifications/)

Then:

+ inside the Karabiner elements app, go to the `Complex Modifications` tab

+ click `add rule`

+ enable the `Change caps_lock to control if pressed with other keys, to escape if pressed alone.` rule

----

#### Spectacle

<img src="https://dl2.macupdate.com/images/icons256/41147.png" align="right" height="150px" />

These are the only commands I use
I have configured them away from the default to not override other hotkeys

 - Fullscreen: cmd + alt + ctrl + p
 - Centre: cmd + alt + ctrl + m
 - Left Half: cmd + alt + ctrl + h
 - Right Half: cmd + alt + ctrl + l
 - Top Half: cmd + alt + ctrl + k
 - Bottom Half: cmd + alt + ctrl + j

Ensure in **`> System Preferences > Security`** you have allowed Spectacle control to your computer

----

#### Iterm2

<img src="https://upload.wikimedia.org/wikipedia/en/d/d7/ITerm2-icon.png" align="right" height="150px" />

**`> Preferences (cmd + ,) > General`**
Untick "Confirm closing multiple sessions"
Untick "Confirm Quit iTerm2"

**`> Preferences > Profiles > General > Working directory`**
Select Reuse previous session's directory

**`> Preferences > Profiles > Window > Settings For New windows`**
Columns: 250, Rows: 100 - For a full screen terminal window each session

----

#### Zsh

The modern shell supported by an [awesome community](http://ohmyz.sh/)

See installation of my config [below](https://github.com/shouston3/my-config#config-installation)

----

#### Vim

See installation of my config [below](https://github.com/shouston3/my-config#config-installation)

I currently use `MacVim` in the terminal `v 8.0`

This can be installed with:

```bash
brew install macvim
```

I open `vim` in the terminal with `mvim -v` which has been aliased to `alias m='mvim -v'`

----

#### Homebrew

Follow instructions here: http://brew.sh

This is what I ran:

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

----

#### Git

```bash
brew install git
```

Cache your git credentials by running:

`git config --global credential.helper osxkeychain`

`git config --global user.name <yourname>`
`git config --global user.email <your@email.com>`

_Note:_ if you have two factor authentication, your password will be your pa-key


You should also globally ignore your `.DS_Store`, this can be done with:

```bash
echo ".DS_Store" > ~/.gitignore_globalgit
config --global core.excludesfile ~/.gitignore_global
```

For a more concise output of `$ gb` (see [here](https://stackoverflow.com/a/48370253)) run the following command:

```bash
git config --global pager.branch false
```

----

If you are looking for a git diff visualisation tool, I would recommend [Source Tree](https://www.sourcetreeapp.com/)

But if you are using `vim`, there is an amazing built in tool that can do this for you.

Everything you need to know about using the tool can be found in [this concise Stack Overflow answer](https://vi.stackexchange.com/a/626)

To get set up run the following commands:

```bash
# Sets vimdiff as the tool to use when you type `git difftool`
git config --global diff.tool vimdiff

# Skip intermediary prompt step to get this running
git config --global difftool.prompt false

# add an alias so that you can get up and running by just typing `git d`
git config --global alias.d difftool
```

----

#### Sass

`gem install sass`

If you get a permissions error, change ownership of that directory

`sudo chown -R $(whoami) /Library/Ruby/Gems/2.0.0` (or whatever ruby version you have)

Then run the command again

----

#### Node

You should install node with nvm, since then you will have more control over which version you are using.

Install it with:

`curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.32.1/install.sh | bash`
(taken from [nvm](https://github.com/creationix/nvm))

Check out the most recent version of node [here](https://nodejs.org/en/) and install it

For me it was:

```bash
nvm install 6.9`
```

Once installed you can update npm to the latest version by running:

```bash
npm install npm@latest -g
```

----

#### Elixir

As simple as:

```bash
brew install elixir
```

I've also installed [Phoenix](http://www.phoenixframework.org/) along side this

For the most up to date installation instructions see [here](http://www.phoenixframework.org/docs/installation#section-phoenix)

It can be installed with:

```bash
mix archive.install https://github.com/phoenixframework/archives/raw/master/phoenix_new.ez
```

----

#### Python

Although mac comes with `python`, I would recommend upgrading to python3, also we don't have `pip` and other python related tools

Get these by running:

```bash
brew install python3
pip3 install --upgrade pip setuptools wheel
```

----

#### Postgres

```bash
brew update
brew install postgres
createdb `whoami``
```

Start the postgres server: `postgres -D /usr/local/var/postgres`

In a new terminal window run: `psql`

I would also recommend using a gui for visualising your database, [Postico](https://eggerapps.at/postico/) would be my choice

You can install it by clicking the download link [here](https://eggerapps.at/postico/) and following the download instructions

----

#### Redis

`brew install redis`

Start the redis server: `redis-server`

In a new terminal window run: `redis-cli`

Now type `ping` and it should respond `pong`

----

#### Heroku toolbelt

As simple as

```bash
brew install heroku
```

#### Grip

If looking for a gui markdown previewer, look at using [haroopad](http://pad.haroopress.com)

I personally don't like guis and want something I can run from the terminal

Install [Grip](https://github.com/joeyespo/grip) with:

```bash
brew install grip
```

#### Misc

<img src="http://core0.staticworld.net/images/article/2013/10/system-preferences-gallery-100065979-large.png" align="right" height="150px" />

`> System Preferences > Trackpad`

Tick: `Tap to click`

To get rid of press and hold character completion, run:

```bash
defaults write -g ApplePressAndHoldEnabled -bool false
```

Hide the dock by right clicking it and selecting: `Turn hiding on`

My key repeat settings found in `System Preferences > Keyboard` are:

+ Key Repeat: `fast`est
+ Delay Until Repeat: `Short`est

#### Config installation

My config can be installed with the following command

```bash
curl -sSL https://raw.githubusercontent.com/shouston3/my-config/readme-refactor/script.sh | bash
```

----

Now your set up with exactly my configuration!

If you think I have missed anything out, or should be doing something differently let me know in an [issue](https://github.com/shouston3/my-config/issues)

Or through gitter - [![gitter badge](https://img.shields.io/badge/gitter-shouston3-brightgreen.svg)](https://gitter.im/shouston3)
