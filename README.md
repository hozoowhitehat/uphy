# uphy
Install docker  xfce 📱💻


docker pull uphy/ubuntu-desktop-jp:20.04

git clone https://github.com/hozoowhitehat/uphy

cd uphy

docker run --rm -p 8080:8080 \
  -v /tmp/pulse:/tmp/pulse \
  -e PULSE_SERVER=unix:/tmp/pulse/native \
  --device /dev/snd \
  --privileged \
  uphy/ubuntu-desktop-jp:20.04



# FIX ERROR


# Pull the image (if not already pulled)
docker pull uphy/ubuntu-desktop-jp:20.04

# Run the container with debugging
docker run --rm -p 8080:8080 \
  -v /tmp/pulse:/tmp/pulse \
  -e PULSE_SERVER=unix:/tmp/pulse/native \
  --device /dev/snd \
  --privileged \
  uphy/ubuntu-desktop-jp:20.04 \
  /bin/bash
