> 一份简单的zsh配置，安装了[oh-my-zsh](https://ohmyz.sh/)

```bash
export ZSH="/home/wimi/.oh-my-zsh"
ZSH_THEME="arrow"
DISABLE_AUTO_UPDATE="true"
DISABLE_UPDATE_PROMPT="true"
DISABLE_LS_COLORS="true"
plugins=(
  git
)
source $ZSH/oh-my-zsh.sh

# local proxy config
proxy(){
  http_proxy="http://127.0.0.1:1087"
  https_proxy="http://127.0.0.1:1087"
  all_proxy="socks5://127.0.0.1:1086"
  echo "HTTP PROXY ON"
}

noproxy(){
  unset http_proxy
  unset https_proxy
  unset all_proxy
  echo "HTTP PROXY OFF"
}

# nodejs config
export PATH="$PATH:/usr/local/node/bin"

# golang config
export PATH="$PATH:/usr/local/go/bin"
export GOPATH="$HOME/go"
export PATH="$GOPATH/bin:$PATH"
export GOPROXY=goproxy.cn
export GO111MODULE=on
```