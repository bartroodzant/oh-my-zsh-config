# oh-my-zsh-config

## Zsh installation

Install zsh:

    sudo apt install zsh

Set zsh as default shell:

    chsh -s /usr/bin/zsh $USER

Log out and log back in to apply the changes. To check the shell use:

    echo $SHELL

It should say `/usr/bin/zsh`

## Oh-my-zsh installation

Install Wget and Git if not already installed:

    apt install wget git

Download the oh-my-zsh installer and execute it:

    wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | zsh

Copy the .zshrc file to your home folder:

    cp ./configs/.zshrc ~/.zshrc

Reload the zsh config:

    source ~/.zshrc

## Powerlevel10k installation

Install the recommended [Meslo](https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k) font variants

Install powerlevel10k theme using oh-my-zsh:

    git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

Restart zsh and you should get a configuration screen for powerlevel10k.
Either go through the configuration screen or use my configuration.

### Sources

[How to forge](https://www.howtoforge.com/tutorial/how-to-setup-zsh-and-oh-my-zsh-on-linux/)

[Powerlevel10k's page](https://github.com/romkatv/powerlevel10k)