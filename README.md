# Style your MAC Shell

To style your shell and have a better overview of your Git projects, follow the steps in the instructions.

![Preview](img/preview.png)

# Instructions

Download iTerm2

https://iterm2.com/

## Shell

Install oh my zsh

https://ohmyz.sh/

```shell
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Plugins

Install plugins and add to ~/.zshrc

https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins

```
$ nano ~/.zshrc
// or
$ vi ~/.zshrc
```

```
plugins=(
git
vscode
...add more...
)
```

## Fonts

Donwload recommended fonts and install with double click.

Follow this link:

https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k

## Theme

https://github.com/romkatv/powerlevel10k

```bash
$ git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
$ echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
```

Now is the time to configure

```bash
p10k configure
```

![Config](img/config.png)

Follow the steps and set everything as you want. That's it.

# Integrate in Mac Terminal

![Mac](img/terminal.png)

Open settings and change font in `MesloLGS NF`

# Integrate in VSC

Open settings in VSC (Visual Studio Code)

Go to Terminal/Console, scroll down to settings.json and click on it

![VSCODE](img/vscode.png)

Add following lines on top in settings under Terminal

https://code.visualstudio.com/docs/editor/integrated-terminal

```json
  "terminal.integrated.fontFamily": "MesloLGS NF",
  "terminal.integrated.profiles.osx": {
    "my-zsh": {
      "path": "zsh",
      "args": ["-l"]
    }
  }
  "terminal.integrated.defaultProfile.osx": "my-zsh"
```

# Integrate in Apache Netbeans

![Apache Netbeans](img/netbeans.png)

Go to Terminal settings and change font to `MesloLGS NF`