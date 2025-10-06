Before installing virtual environment
make sure u install ubuntu in termux first 


Looks like Python 3.12 actually Works!! U have to create a virtual environment so here is the guide:


To run ComfyUI in a separate environment on Termux with Python 3.10.11, follow these steps:


---

1. Install Required Packages

First, ensure your Termux is updated and install necessary packages:

apt update -y && apt upgrade -y
apt install python3-full git ffmpeg


---

2. Install & Setup a Virtual Environment

Create and activate a virtual environment:

python3 -m venv comfyui-env
source comfyui-env/bin/activate










Holy Moly!!!! This Works on 12gb Ram!!!

sorry guys and gals fooocus is broken we haven't had an update in 6 months I hope fooocus isn't dead I really liked it but I tried running it and it just sits on waiting to begin task¿

1> pkg update -y && pkg install wget curl proot tar -y && wget https://raw.githubusercontent.com/AndronixApp/AndronixOrigin/master/Installer/Ubuntu22/ubuntu22.sh -O ubuntu22.sh && chmod +x ubuntu22.sh && bash ubuntu22.sh

2> apt update && apt upgrade -y && apt-get install curl git gcc make build-essential python3 python3-dev python3-pip python3-venv python-is-python3 -y && apt dist-upgrade -y && apt install wget && apt-get install libgl1 libglib2.0-0 libsm6 libxrender1 libxext6 -y && apt-get install google-perftools &&
apt install libgoogle-perftools-dev && pip install moviepy==1.0.3 && apt-get install -y build-essential python3-dev python3-setuptools make cmake && apt-get install -y ffmpeg libavcodec-dev libavfilter-dev libavformat-dev libavutil-dev

4> git clone https://github.com/lllyasviel/Fooocus

5> cd Fooocus

'Fix' the issue with Python running in PRoot

export ANDROID_DATA=anything

6> pip install -r requirements_versions.txt

WHEN YOU RESTART TERMUX

cd ubuntu-in-termux && ./startubuntu.sh

cd Fooocus && python launch.py --preset realistic --always-offload-from-vram --vae-in-cpu --clip-in-fp8-e4m3fn --attention-split --always-cpu --all-in-fp16 --unet-in-fp8-e4m3fn --disable-server-log --disable-async-cuda-allocation

cd Fooocus && python launch.py --preset anime --vae-in-bf16 --always-offload-from-vram --vae-in-cpu --clip-in-fp8-e4m3fn --attention-split --always-cpu --all-in-fp16 --unet-in-fp8-e4m3fn --preview-option taesd --disable-server-log --disable-async-cuda-allocation