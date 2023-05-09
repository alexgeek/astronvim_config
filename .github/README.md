# AstroNvim User Configuration Example

A user configuration template for [AstroNvim](https://github.com/AstroNvim/AstroNvim)

## 🛠️ Installation

#### Make a backup of your current nvim and shared folder

```shell
mv ~/.config/nvim ~/.config/nvim.bak
mv ~/.local/share/nvim ~/.local/share/nvim.bak
```

#### Clone AstroNvim

```shell
git clone https://github.com/AstroNvim/AstroNvim ~/.config/nvim
```

#### Create a new user repository from this template

Press the "Use this template" button above to create a new repository to store your user configuration.

You can also just clone this repository directly if you do not want to track your user configuration in GitHub.

#### Clone the repository

```shell
git clone https://github.com/alexgeek/astronvim_config ~/.config/nvim/lua/user
# or SSH
git clone git@github.com:alexgeek/astronvim_config.git ~/.config/nvim/lua/user
```

#### Start Neovim

```shell
nvim
```


#### Troubleshooting

https://neovim.discourse.group/t/where-do-language-server-logs-go/1303/3

```lua
:checkhealth mason
```

Logs:
```sh
ls ~/.cache/nvim/
ls ~/.local/state/nvim/lsp.log
```

#### Dependencies

```sh
cargo install ripgrep
cargo install tree-sitter-cli
sudo apt install -y lua5.1
sudo apt install -y php
sudo apt install -y julia
sudo apt install -y php-cli
sudo apt install -y gem
sudo apt install -y ruby

sudo npm cache clean -f
sudo npm install -g n
sudo n stable
sudo n latest

curl -sS https://getcomposer.org/installer -o /tmp/composer-setup.php
HASH=`curl -sS https://composer.github.io/installer.sig`
php -r "if (hash_file('SHA384', '/tmp/composer-setup.php') === '$HASH') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
sudo php /tmp/composer-setup.php --install-dir=/usr/local/bin --filename=composer

go install github.com/dundee/gdu/v5/cmd/gdu@latest
cargo install bottom --locked

```
