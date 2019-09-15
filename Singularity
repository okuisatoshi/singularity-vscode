Bootstrap:docker
From: ubuntu:bionic

%post

apt-get update
apt-get install -y wget

wget https://go.microsoft.com/fwlink/?LinkID=760868 -O /tmp/vscode.deb

dpkg -i /tmp/vscode.deb || true
apt-get install -y -f
apt-get install -y x11-common libx11-xcb1 libasound2
apt-get clean

$runscript

/usr/bin/code









