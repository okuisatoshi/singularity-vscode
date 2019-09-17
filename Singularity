Bootstrap:docker
From: ubuntu:bionic


%post

apt-get update
apt-get install -y wget

wget https://go.microsoft.com/fwlink/?LinkID=760868 -O /tmp/vscode.deb

dpkg -i /tmp/vscode.deb || true
apt-get install -y -f
apt-get install -y libx11-xcb1 libasound2 # x11-common
apt-get clean

mkdir /run/user/683402166
chmod a+rwx /run/user
chmod a+rwx /run/user/683402166

%runscript

/usr/bin/code









