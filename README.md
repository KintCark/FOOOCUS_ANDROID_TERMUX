Holy Moly!!!! This Works on 12gb Ram!!!

# FOOOCUS_ANDROID_TERMUX

The New 2.5.0 Update Works On 12gb Ram Cpu Mode
I had to use developer advanced settings to use this u can use sd1.5 and sdxl also change refiner to separate mode and
use sd15 2gb pruned models only, 4gb idk about 3gb but 4gb and Up won't work they run up ram. also in developer tab disable soft controller and enable skip preprocessors,I can make 7:9 images with these settings,also put the termux app and stargon browser app in split screen,that's the only way you can run without crash,some reason sdxl only works when termux is in the foreground, u can't run sdxl with termux as background process.
now I can use fooocus officially on my phone!



1> pkg updated && pkg upgrade -y && termux-setup-storage &&
pkg install wget -y && pkg install git -y && pkg install proot -y &&
cd ~ && git clone https://github.com/MFDGaming/ubuntu-in-termux.git && cd ubuntu-in-termux && chmod +x ubuntu.sh && ./ubuntu.sh -y && ./startubuntu.sh 

2> apt update && apt upgrade -y && apt-get install curl git gcc make build-essential python3 python3-dev python3-distutils python3-pip python3-venv python-is-python3 -y 

3> apt-get install libgl1 libglib2.0-0 libsm6 libxrender1 libxext6 -y

4> git clone https://github.com/lllyasviel/Fooocus

5> cd Fooocus


'Fix' the issue with Python running in PRoot

export ANDROID_DATA=anything 



6> pip install -r requirements_versions.txt

WHEN YOU RESTART TERMUX 

cd ubuntu-in-termux && ./startubuntu.sh

cd Fooocus && python launch.py --preset realistic --vae-in-bf16 --always-offload-from-vram --vae-in-cpu --clip-in-fp8-e4m3fn --attention-split --always-cpu --all-in-fp16 --unet-in-fp8-e4m3fn --preview-option taesd --disable-server-log --disable-async-cuda-allocation

cd Fooocus && python launch.py --preset anime --vae-in-bf16 --always-offload-from-vram --vae-in-cpu --clip-in-fp8-e4m3fn --attention-split --always-cpu --all-in-fp16 --unet-in-fp8-e4m3fn --preview-option taesd --disable-server-log --disable-async-cuda-allocation
