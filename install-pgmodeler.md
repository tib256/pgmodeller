Install
sudo apt-get update
cd
wget https://codeload.github.com/pgmodeler/pgmodeler/tar.gz/v0.9.2
tar -xvzf v0.9.2
mv pgmodeler-0.9.2/ pgmodeler
cd pgmodeler
git clone https://github.com/pgmodeler/plugins assuming git is already installed
install postgresql (how to install in different guide)
sudo apt-get install make g++ qt5-qmake libxml2-dev libpq-dev pkg-config libqt5svg5-dev qttools5-dev
sudo apt-get install qt5-default libqt5svg5
cd ~/pgmodeler
qmake pgmodeler.pro
make -j8 -j8 means use all 8 cpu cores, use only "make" if not sure
sudo make install
run using '/usr/local/bin/pgmodeler'
cleanup
sudo apt-get remove --purge -y make g++ qt5-qmake libxml2-dev pkg-config libqt5svg5-dev
sudo apt-get autoremove
Desktop Entry
sudo pico /usr/share/applications/pgmodeler.desktop

paste following with correct Icon path

[Desktop Entry]
Name=pgModeler
GenericName=PostgreSQL Database Modeler
Comment=Program with nice Qt interface for visual modeling PostgreSQL on Entity Relationship Diagram
Exec=pgmodeler
Icon=/home/varungpt/pgmodeler/main/res/windows_ico.ico
Terminal=false
Type=Application
Categories=Qt;Database;Development;

Blogs :
https://hub.docker.com/r/kayvan/pgmodeler/dockerfile
https://medium.com/@mglaving/how-to-run-pgmodeler-0-9-2-on-raspberry-pi-4-ebbca63173cc
https://www.muehlencord.de/wordpress/2016/01/28/build-pgmodeler-from-source/
https://www.simonholywell.com/post/2016/10/install-pgmodeler-ubuntu/
https://pgmodeler.io/support/installation
