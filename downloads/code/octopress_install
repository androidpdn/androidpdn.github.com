sudo apt-get install bash curl git-core -y
sudo apt-get install build-essential bison openssl libreadline6 libreadline6-dev zlib1g zlib1g-dev libssl-dev libyaml-dev libsqlite3-0 libsqlite3-dev sqlite3 libxml2-dev libxslt-dev autoconf libc6-dev ncurses-dev automake -y
bash < <(curl -s https://rvm.beginrescueend.com/install/rvm)
echo '[[ -s "$HOME/.rvm/scripts/rvm" ]] && . "$HOME/.rvm/scripts/rvm" # Load RVM function' >> ~/.bash_profile
source .bash_profile
rvm pkg install openssl
rvm --skip-autoreconf pkg install iconv
rvm install 1.9.2 -C --with-openssl-dir=$HOME/.rvm/usr,--with-iconv-dir=$HOME/.rvm/usr
rvm use 1.9.2 --default
rvm reload
rvm rubygems latest
gem install bundler
cd
git clone git://github.com/imathis/octopress.git octopress
cd octopress
bundle install
rake install
