THIS WORKS ON 8GB RAM!!! DON'T DISABLE PHANTOM PROCESSOR KILLER DOING THIS WILL MAKE ALL STABLE DIFFUSION TERMUX CRASH!!!


# FOOOCUS_ANDROID_TERMUX
I've done it once again we can use fooocus on Android yes sdxl works!!!
also make sure u have high end phone 12gb ram minimum!! and enable developer option 
and disable background processes to free more ram!!

YOU NEED THIS TERMUX MOD VERSION THIS IS THE ONE I USED!


https://github.com/KitsunedFox/termux-monet


1> pkg updated && pkg upgrade -y && termux-setup-storage &&
pkg install wget -y && pkg install git -y && pkg install proot -y &&
cd ~ && git clone https://github.com/MFDGaming/ubuntu-in-termux.git && cd ubuntu-in-termux && chmod +x ubuntu.sh && ./ubuntu.sh -y && ./startubuntu.sh 

2> apt update && apt upgrade -y && apt-get install curl git gcc make build-essential python3 python3-dev python3-distutils python3-pip python3-venv python-is-python3 -y 

3> apt-get install libgl1 libglib2.0-0 libsm6 libxrender1 libxext6 -y

4> git clone https://github.com/lllyasviel/Fooocus

5> cd Fooocus

6> pip install -r requirements_versions.txt

7> python launch.py --preset realistic --vae-in-fp16 --always-offload-from-vram --vae-in-cpu --clip-in-fp8-e4m3fn --attention-split --always-cpu  --all-in-fp16 --unet-in-fp8-e5m2 --preview-option taesd --disable-server-log --disable-async-cuda-allocation

7> python launch.py --preset anime --vae-in-fp16 --always-offload-from-vram --vae-in-cpu --clip-in-fp8-e4m3fn --attention-split --always-cpu  --all-in-fp16 --unet-in-fp8-e5m2 --preview-option taesd --disable-server-log --disable-async-cuda-allocation

WHEN YOU RESTART TERMUX 

cd ubuntu-in-termux && ./startubuntu.sh

cd Fooocus

python launch.py --preset realistic --vae-in-fp16 --always-offload-from-vram --vae-in-cpu --clip-in-fp8-e4m3fn --attention-split --always-cpu  --all-in-fp16 --unet-in-fp8-e5m2 --preview-option taesd --disable-server-log --disable-async-cuda-allocation

python launch.py --preset anime --vae-in-fp16 --always-offload-from-vram --vae-in-cpu --clip-in-fp8-e4m3fn --attention-split --always-cpu  --all-in-fp16 --unet-in-fp8-e5m2 --preview-option taesd --disable-server-log --disable-async-cuda-allocation
