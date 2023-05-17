![image](https://github.com/DavideBri/shell-superMegaFiga/assets/70480082/7a174ecd-d781-47f3-b39d-e798c63e02dd)

The purpose of this repository is to serve as a backup for the configuration file of my zsh shell. 
In case you would like to recreate it, you may refer to the step-by-step guide provided below.


# How to Install shell-SMF

Prerequisites:
A Unix-like operating system, git, curl, wget, pip3

```
sudo apt install git curl wget
sudo apt install python3-pip
``` 
> reload and resart the program when installing or modifing the config file.

## terminator 📺
  
  install it from the snap store.

  Go in the `$HOME/.config/terminator/plugins` folder, If doesnt exist run:

  `mkdir -p $HOME/.config/terminator/plugins`

  Now install the TerminatorThemes run:

  ```
  wget https://git.io/v5Zww -O $HOME"/.config/terminator/plugins/terminator-themes.py"
  ```

  Check the **TerminatorThemes** option under terminator > preferences > plugins.
  Open the terminator context menu and select Themes.
  Select you favorite (dracula) theme and click install.

  Now paste the `terminator/` folder into the `./config/`
  ```
  mv terminator/ ../.config/
  ```
  🎉 DONE! (1/4)

  > TIP to open the contex menu click the scroll wheel on the terminal

  ### Terminator Shortcuts

  `CTR+SHIFT+O` split horizontal

  `CTR+SHIFT+E` split vertical

  `CTR+SHIFT+W` close current terminal


## zsh 🔥

install zsh
```
sudo apt install zsh
``` 
 Now paste the `.zshrc` file into the old one
  ```
  mv .zshrc ../.zshrc
  ```
> Dont worry about warning about plugins

You succesfully imported also aliases such as
- update
- purge
- forecast
- htop ( but is bytop )
- upload [file] ( upload a file to tmp.sh )

🎉 DONE! (2/4)

## oh-my-zsh 👀

install it from:
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

  the theme installed are:
  - **sudo**, double `esc` will redo the previus prompt with sudo
  - **git**, for git shortcut
  - **zsh-higligthing**, self explanatory

  install the zsh-higligthing plugin:
  ```
  git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
  ```

🎉 DONE! (3/4)

## powerline10k 🔋

install the oh-my-zsh theme by running:

```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

press `q` when the wizard install pop ups.
Now paste the `.p10k.zsh` file into the old one
  
  ```
  mv .p10k.zsh ../.p10k.zsh
  ```
DONE! (4/4) 🥳🥳

enjoy the SMF-shell
