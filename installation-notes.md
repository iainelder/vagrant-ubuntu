# Installation Notes

## VS Code Extensions

```bash
code --list-extensions
```

```text
4ops.terraform
bdavs.expect
bierner.markdown-preview-github-styles
Boto3typed.boto3-ide
bungcip.better-toml
eamodio.gitlens
eastman.vscode-cfn-nag
eriklynd.json-tools
hashicorp.hcl
hashicorp.terraform
janisdd.vscode-edit-csv
jeff-hykin.macro-commander
joaompinto.vscode-graphviz
kddejong.vscode-cfn-lint
marvhen.reflow-markdown
MS-CEINTL.vscode-language-pack-es
ms-python.isort
ms-python.python
ms-python.vscode-pylance
ms-toolsai.jupyter
ms-toolsai.vscode-jupyter-cell-tags
ms-toolsai.vscode-jupyter-slideshow
mushan.vscode-paste-image
redhat.vscode-yaml
seanwu.vscode-qt-for-python
takezoe.vscode-csv-markdown
trond-snekvik.simple-rst
tshino.kb-macro
```

## Apt packages

```bash
comm -23 \
<(apt-mark showmanual | sort -u) \
<(gzip -dc /var/log/installer/initial-status.gz | sed -n 's/^Package: //p' | sort -u)
```

```text
1password
ack
aha
apt-file
apt-transport-https
atop
auditd
autoconf
autofirma
awsvpnclient
azure-cli
azuredatastudio
bats
bison
blueman
bpfcc-tools
build-essential
catfish
cnijfilter2
cnijfilter-common
cnijfilter-mg2500series
cobang
code
composer
cronopete
crudini
csvtool
curl
datamash
dbeaver-ce
db-util
default-jre
diff-so-fancy
discord
docker.io
dosbox
dvc
epson-inkjet-printer-escpr
epson-printer-utility
evolution
evolution-ews
expandrive
expect
ffmpeg
flameshot
g++
gcc
gcm
git
git-extras
git-flow
gnome-clocks
gnome-sound-recorder
gnucash
gnumeric
gnupg2
gnuplot
golang-1.15
golang-1.16
golang-go
google-chrome-stable
gpw
graphviz
graphviz-doc
grepcidr
gron
gzdoom
htop
hunspell-en-au
hunspell-en-ca
hunspell-en-gb
hunspell-en-za
hyphen-en-ca
hyphen-en-gb
iftop
imagescan
imagescan-plugin-gt-s650
imagescan-plugin-networkscan
imagescan-plugin-ocr-engine
ipython3
jo
jq
kitty
kubectl
libbz2-dev
libdb-dev
libemail-outlook-message-perl
libffi-dev
libgdbm-dev
libglade2-0
liblzma-dev
libncurses5-dev
libncursesw5-dev
libreadline-dev
libreoffice-help-en-gb
libreoffice-l10n-en-gb
libreoffice-l10n-en-za
libsecret-tools
libsqlite3-dev
libssl-dev
libxml2-dev
libxml2-utils
libxmlsec1-dev
libyaml-dev
linux-hwe-5.8-headers-5.8.0-44
llvm
local
make
mhonarc
miller
moreutils
mpack
mplayer
mssql-tools
mutt
mypaint
mysql-client-core-8.0
mythes-en-au
ncat
netatalk
netcat
net-tools
network-manager-l2tp-gnome
nmap
nodejs
nomacs
openrazer-meta
opera-stable
p7zip-full
packages-microsoft-prod
packer
pandoc
pdd
php7.4
php-curl
php-mbstring
php-xml
php-yaml
postgresql-client-12
postgresql-client-common
powershell
pv
python3-pip
python3-pydrive
python3-pyotp
python3-venv
python3-wheel
q-text-as-data
ripgrep
rocketchat
scangearmp2
scangearmp-common
scangearmp-mg2500series
scrcpy
session-manager-plugin
simplescreenrecorder
smartmontools
smemstat
sox
spotify-client
sqlite3
steam:i386
stow
stress-ng
strongswan
tcl
tcl-thread
tcptrack
teams
texlive-fonts-recommended
texlive-latex-base
texlive-plain-generic
thunderbird-locale-en-gb
thunderbird-locale-es-ar
tidy
tk-dev
traceroute
tree
typora
unixodbc-dev
unp
unrar
vagrant
vim
virtualbox-6.1
whois
workspacesclient
xclip
zlib1g-dev
zoom
```

## Pipx packages

```bash
pipx list --short
```

```
ankipandas 0.3.10
asciinema 2.2.0
athenacli 1.6.8
aws-export-credentials 0.13.0
aws-gate 0.11.2
aws-org-inventory 0.5.2.post1
aws-org-tree 0.2.0
aws-sam-cli 1.61.0
aws-ssm-tree 0.2.1
aws-sso-util 4.29.0
aws-utilities 1.3.1
aws-whoami 1.2.0
aws2-wrap 1.3.0
awscfncli2 3.1.1
black 22.10.0
cfn-flip 1.3.0
cfn-lint 0.69.1
cfripper 1.13.1
cookiecutter 2.1.1
cruft 2.11.1
csvkit 1.0.7
docker-compose 1.29.2
ec2instanceconnectcli 1.0.2
git-filter-repo 2.38.0
git-remote-codecommit 1.16
identify 2.5.8
ipython 8.6.0
isort 5.10.1
jc 1.22.1
jtbl 1.4.0
jupyterlab 3.5.0
lastversion 2.4.5
litecli 1.9.0
mitmproxy 8.0.0
parliament 1.6.1
pew 1.2.0
pipenv 2022.10.25
poetry 1.2.2
pre-commit 2.20.0
procpath 1.6.1
psgdemos 1.12.1
py-spy 0.3.14
pylint 2.15.5
s3-tree 0.1.0
sceptre 3.2.0
sqlfluff 1.4.0
sqlite-utils 3.30
tabulate 0.9.0
taskcat 0.9.33
tox 3.27.0
trufflehog 2.2.1
venvs 7.3.2
virtualenvwrapper 4.8.4
visidata 2.10.2
vwlogin 0.1.2
yamllint 1.28.0
youtube-dl 2021.12.17
```
