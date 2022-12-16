# If you come from bash you might have to change your $PATH.

# export PATH=$HOME/bin:/usr/local/bin:$PATH

# Path to your oh-my-zsh installation.

export ZSH="$HOME/.oh-my-zsh"

# Set name of the theme to load --- if set to "random", it will

# load a random theme each time oh-my-zsh is loaded, in which case,

# to know which specific one was loaded, run: echo $RANDOM_THEME

# See https://github.com/ohmyzsh/ohmyzsh/wiki/Themes

ZSH_THEME="robbyrussell"

# Set list of themes to pick from when loading at random

# Setting this variable when ZSH_THEME=random will cause zsh to load

# a theme from this variable instead of looking in $ZSH/themes/

# If set to an empty array, this variable will have no effect.

# ZSH_THEME_RANDOM_CANDIDATES=( "robbyrussell" "agnoster" )

# Uncomment the following line to use case-sensitive completion.

# CASE_SENSITIVE="true"

# Uncomment the following line to use hyphen-insensitive completion.

# Case-sensitive completion must be off. \_ and - will be interchangeable.

# HYPHEN_INSENSITIVE="true"

# Uncomment one of the following lines to change the auto-update behavior

# zstyle ':omz:update' mode disabled # disable automatic updates

# zstyle ':omz:update' mode auto # update automatically without asking

# zstyle ':omz:update' mode reminder # just remind me to update when it's time

# Uncomment the following line to change how often to auto-update (in days).

# zstyle ':omz:update' frequency 13

# Uncomment the following line if pasting URLs and other text is messed up.

# DISABLE_MAGIC_FUNCTIONS="true"

# Uncomment the following line to disable colors in ls.

# DISABLE_LS_COLORS="true"

# Uncomment the following line to disable auto-setting terminal title.

# DISABLE_AUTO_TITLE="true"

# Uncomment the following line to enable command auto-correction.

# ENABLE_CORRECTION="true"

# Uncomment the following line to display red dots whilst waiting for completion.

# You can also set it to another string to have that shown instead of the default red dots.

# e.g. COMPLETION_WAITING_DOTS="%F{yellow}waiting...%f"

# Caution: this setting can cause issues with multiline prompts in zsh < 5.7.1 (see #5765)

# COMPLETION_WAITING_DOTS="true"

# Uncomment the following line if you want to disable marking untracked files

# under VCS as dirty. This makes repository status check for large repositories

# much, much faster.

# DISABLE_UNTRACKED_FILES_DIRTY="true"

# Uncomment the following line if you want to change the command execution time

# stamp shown in the history command output.

# You can set one of the optional three formats:

# "mm/dd/yyyy"|"dd.mm.yyyy"|"yyyy-mm-dd"

# or set a custom format using the strftime function format specifications,

# see 'man strftime' for details.

# HIST_STAMPS="mm/dd/yyyy"

# Would you like to use another custom folder than $ZSH/custom?

# ZSH_CUSTOM=/path/to/new-custom-folder

# Which plugins would you like to load?

# Standard plugins can be found in $ZSH/plugins/

# Custom plugins may be added to $ZSH_CUSTOM/plugins/

# Example format: plugins=(rails git textmate ruby lighthouse)

# Add wisely, as too many plugins slow down shell startup.

plugins=(
git
zsh-syntax-highlighting
zsh-autosuggestions

)

source $ZSH/oh-my-zsh.sh

# User configuration

# export MANPATH="/usr/local/man:$MANPATH"

# You may need to manually set your language environment

# export LANG=en_US.UTF-8

# Preferred editor for local and remote sessions

# if [[-n $SSH_CONNECTION]]; then

# export EDITOR='vim'

# else

# export EDITOR='mvim'

# fi

# Compilation flags

# export ARCHFLAGS="-arch x86_64"

# Set personal aliases, overriding those provided by oh-my-zsh libs,

# plugins, and themes. Aliases can be placed here, though oh-my-zsh

# users are encouraged to define aliases within the ZSH_CUSTOM folder.

# For a full list of active aliases, run `alias`.

#

# Example aliases

# alias zshconfig="mate ~/.zshrc"

# alias ohmyzsh="mate ~/.oh-my-zsh"

NC='\033[0m' # Text Reset

# Regular Colors

Black='\033[0;30m' # Black
Red='\033[0;31m' # Red
Green='\033[0;32m' # Green
Yellow='\033[0;33m' # Yellow
Blue='\033[0;34m' # Blue
Purple='\033[0;35m' # Purple
Cyan='\033[0;36m' # Cyan
White='\033[0;37m' # White

# %n : 유저이름

# %m : 기계이름

# %1~ symbol means the current working directory path where the ~ strips the $HOME directory location.

# %~ : 디렉터리

# %1~ : 디렉터리 끝

PROMPT='%n~$'
PROMPT='%F{125}%n%f' # F 색변환 f 색변환 종료
PROMPT='%F{125}%1~%f'

# git 보이게 설정

function parse_git_branch() {
git branch 2> /dev/null | sed -n -e 's/^\* \(.\*\)/\1/p'
}
COLOR_DEF=$'\e[0m'
COLOR_USR=$'\e[38;5;243m'
COLOR_DIR=$'\e[33;35;115m'
COLOR_GIT=$'\e[38;5;39m'
setopt PROMPT_SUBST

# %{ %} 이걸로 감싸야 자동완성이 깨지지 않는다

export PROMPT='%{${COLOR_DIR}%}%1~ %{${COLOR_GIT}%}$(parse_git_branch)%{${COLOR_DEF}%} <%F{red}<%f '
