## My Mac Setup

This repo contains info on all the apps / tools / settings I use on my Mac.

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [OS Settings](#os-settings)
  - [Desktop](#desktop)
  - [Finder](#finder)
  - [Dock](#dock)
- [Quick Launching](#quick-launching)
- [Homebrew](#homebrew)
  - [Homebrew](#homebrew-1)
- [Window Management](#window-management)
- [Menu Bar Utilities](#menu-bar-utilities)
  - [Hidden Bar](#hidden-bar)
  - [System Stats Widgets](#system-stats-widgets)
- [Web Browser](#web-browser)
- [Other Apps I Use Daily](#other-apps-i-use-daily)
  - [Docker](#docker)
- [Terminal](#terminal)
  - [Shell](#shell)
  - [Github SSH Setup](#github-ssh-setup)
    - [Other command line tools I use](#other-command-line-tools-i-use)
- [VS Code](#VS-Code-Settings)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## OS Settings

These are my preferred settings for `Desktop`, `Finder` and the `Dock`.

### Desktop

I don't like the new Desktop, Stage Manager or Widget features in Sonoma, so I disable them.

* System Preferences
  * Desktop & Dock
    * Desktop & Stage Manager
      * Show Items
        * On Desktop -> uncheck
        * In Stage Manager -> uncheck
      * Click wallpaper to reveal desktop -> Only in Stage Manager
      * Stage Manager -> uncheck
      * Widgets
        * On Desktop -> uncheck
        * In Stage Manager -> uncheck

### Finder

* Finder -> Preferences
  * General -> Show these on the desktop -> Select None
      * I try to keep my desktop completely clean.
  * General -> New Finder windows show -> Home Folder
      * I prefer to see my home folder in each new finder window instead of recent documents
  * Advanced -> Show all filename extensions -> Yes
  * Advanced -> Show warning before changing an extension -> No
  * Advanced -> When performing a search -> Search the current folder
* View
  * Show Status Bar
  * Show Path Bar
  * Show Tab Bar

### Dock

I don't use the Dock at all. It takes up screen space, and I can use RayCast to launch apps and AltTab to switch between apps. I make the dock as small as possible and auto hide it.

* System Preferences
  * Desktop & Dock
    * Size -> Small as possible
    * Position on screen -> Left
    * Automatically hide and show the Dock -> Yes
    * Animate opening applications -> No
    * Show suggested and recent apps in the Dock -> No


## Homebrew

### Homebrew

[Homebrew](https://brew.sh/) allows us to install tools and apps from the command line.


## Window Management

I use [rectangle](https://rectangleapp.com/) to move and resize windows using keyboard shortcuts.

```sh
brew install rectangle
```

## Menu Bar Utilities

### Hidden Bar

If you have several apps running that have menu bar icons, [Hidden Bar](https://github.com/dwarvesf/hidden) will let you choose which ones should be hidden after a timeout. This cleans things up if you have a ton of background apps running.

```sh
brew install hiddenbar
```

### System Stats Widgets

I use [stats](https://github.com/exelban/stats) to see my network traffic, CPU temp / usage and RAM usage at a glance.

```sh
brew install stats
```

## Web Browser

I use the following extensions to protect my privacy while browsing the web:

* Adblocker - [uBlock Origin](https://github.com/gorhill/uBlock)
* Tracker Blocker - [Privacy Badger](https://privacybadger.org/)
  * Firefox now includes tracker blocking, but I leave Privacy Badger enabled.
* [Decentraleyes](https://decentraleyes.org/)
  * Caches CDN links locally and intercepts requests to serve from the cache. Prevents CDNs from tracking you across websites.

## Other Apps I Use Daily

### Docker

There are multiple results when you search `docker` within `brew`. To install Docker desktop:

```sh
brew install --cask docker
```

## Terminal

I prefer [iTerm2](https://iterm2.com/) because:
* Lots of customization options
* Clickable links
* Native OS notifications

There are a lot of options for a terminal replacement, but I've been using iTerm2 for years and it works great for my needs.

Checkout their documentation for more info on what iTerm2 can do: [https://iterm2.com/documentation.html](https://iterm2.com/documentation.html)


```
brew install iterm2
```

Once installed, launch it and customize the settings / preferences to your liking. These are my preferred settings:

* Appearance
  * Theme
    * Minimal
* Profiles
  * Default
      * General -> Working Directory -> Reuse previous session's directory
      * Colors -> Basic Colors -> Foreground -> Lime Green
      * Text -> Font -> Anonymous Pro
          * You can download this font [here](https://www.marksimonson.com/fonts/view/anonymous-pro).
          * I use this font in VS Code as well
      * Text -> Font Size -> 36
          * I use my Macbook to present / teach, so a big font size is important so everyone can see the commands I'm typing
      * Keys -> Key Mappings -> Presets -> Natural Text Editing
          * This allows me to use the [keyboard shortcuts](https://gist.github.com/w3cj/022081eda22081b82c52) I know and love inside of iTerm2

### Shell

Mac now comes with `zsh` as the default [shell](https://en.wikipedia.org/wiki/Comparison_of_command_shells). I've switched to using this with [Oh My Zsh](https://ohmyz.sh/).

#### Load dotfiles

All my dotfiles are stored on [github](https://github.com/Lel3x)
I clone this repo to my machine and copy the files into my home directory.

### Github SSH Setup

* Follow [this guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) to setup an ssh key for github
* Follow [this guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) to add the ssh key to your github account



# VS Code Settings

# Font

* [Anonymous Pro](https://www.marksimonson.com/fonts/view/anonymous-pro)

## Themes/Color

* [Just Black](https://marketplace.visualstudio.com/items?itemName=nur.just-black)
  * See [`editor.tokenColorCustomizations`](#settings) in my VS Code settings for a few modifications I make to the theme.

## Extensions

```
vscode-icons-team.vscode-icons
esbenp.prettier-vscode
vunguyentuan.vscode-postcss
streetsidesoftware.code-spell-checker
yoavbls.pretty-ts-errors
styled-components.vscode-styled-components
bierner.markdown-mermaid
github.codespaces
github.copilot-chat
seyyedkhandon.firacode
tomoki1207.pdf
shd101wyy.markdown-preview-enhanced
```

# Settings
settings.json file <--
