# raspberry-pi-4-mjpg-install

sudo apt-get update

sudo apt-get install libjpeg8-dev

sudo apt-get install imagemagick

sudo apt-get install libv4l-dev

sudo apt-get install cmake

sudo apt-get install git

sudo apt-get install unzip

wget https://github.com/jacksonliam/mjpg-streamer/archive/master.zip

unzip master.zip

cd mjp*g-*

cd mjpg-*

make

sudo make install

cd

/usr/local/bin/mjpg_streamer -i "/usr/local/lib/mjpg-streamer/input_uvc.so -n -f 30 -r 1280x720" -o "/usr/local/lib/mjpg-streamer/output_http.so -p 8080 -w /usr/local/share/mjpg-streamer/www"

http://192.168.60.122:8080/?action=stream
