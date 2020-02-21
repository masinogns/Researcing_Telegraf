Srouce Code Download Page
: https://coderelease.io/github/repository/influxdata/telegraf


Install Go >=1.12 (1.13 recommended)

"""
https://linuxize.com/post/how-to-install-go-on-centos-7/

wget https://dl.google.com/go/go1.13.linux-amd64.tar.gz
sudo tar -C /usr/local -xzf go1.13.linux-amd64.tar.gz

vi ~/.bash_profile
export PATH=$PATH:/usr/local/go/bin

source ~/.bash_profile

mkdir -p ~/go/src/hello


"""

Install dep ==v0.5.0

"""

go get -u github.com/golang/dep/cmd/dep

mkdir -p /data/telegraf/go
cd /data/telegraf/go
mkdir bin src pkg

cd ./src
git clone http://telegraf_source_code-github

cd ./Repository_github
MAKE

$ export GOROOT=/usr/local/go
$ export GOPATH=/data/telegraf/go
$ echo $GOPATH
$ echo $GOROOT

curl https://raw.githubusercontent.com/golang/dep/master/install.sh | sh
/*
root@rlgns_telegraf go]# curl https://raw.githubusercontent.com/golang/dep/master/install.sh | sh
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  5230  100  5230    0     0   5480      0 --:--:-- --:--:-- --:--:--  5476
ARCH = amd64
OS = linux
Will install into /data/telegraf/go/bin
Fetching https://github.com/golang/dep/releases/latest..
Release Tag = v0.5.4
Fetching https://github.com/golang/dep/releases/tag/v0.5.4..
Fetching https://github.com/golang/dep/releases/download/v0.5.4/dep-linux-amd64..
Setting executable permissions.
Moving executable to /data/telegraf/go/bin/dep
*/
/*
"""
