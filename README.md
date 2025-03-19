# uphy
Install docker  xfce 📱💻


git clone https://github.com/hozoowhitehat/uphy

cd uphy

docker run --rm -p 8080:8080 \
  -v /tmp/pulse:/tmp/pulse \
  -e PULSE_SERVER=unix:/tmp/pulse/native \
  --device /dev/snd \
  --privileged \
  uphy/ubuntu-desktop-jp:20.04
