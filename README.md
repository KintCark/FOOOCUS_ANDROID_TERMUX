Holy Moly!!!! This Works on 12gb Ram!!!

# FOOOCUS_ANDROID_TERMUX

The New 2.5.5 Update Works On 12gb Ram Cpu Mode
now I can use fooocus officially on my phone!, download swap file no root app pay the 1 dollar premium fee crank it all the way to 8gb then if u have ram plus feature enable that also ull have 16gb extra swap memory this is one reason fooocus is working 
😉 Enjoy! but warning useing high resolution will make your phone H0T!! you still need developer options it ran fine for first boo y but now it's crashing again so use developer option I can do w 512 h 1024 It gives great sdxl photos for speed.


1> pkg updated && pkg upgrade -y && termux-setup-storage &&
pkg install wget -y && pkg install git -y && pkg install proot -y &&
cd ~ && git clone https://github.com/MFDGaming/ubuntu-in-termux.git && cd ubuntu-in-termux && chmod +x ubuntu.sh && ./ubuntu.sh -y && ./startubuntu.sh 

2> apt update && apt upgrade -y && apt-get install curl git gcc make build-essential python3 python3-dev python3-distutils python3-pip python3-venv python-is-python3 -y 

3> apt-get install libgl1 libglib2.0 libsm6 libxrender1 libxext6 -y

4> git clone https://github.com/lllyasviel/Fooocus

5> cd Fooocus


'Fix' the issue with Python running in PRoot

export ANDROID_DATA=anything 



6> pip install -r requirements_versions.txt --break-system-packages

WHEN YOU RESTART TERMUX 

cd ubuntu-in-termux && ./startubuntu.sh

cd Fooocus && python launch.py --preset realistic --vae-in-fp16 --always-offload-from-vram --vae-in-cpu --clip-in-fp8-e4m3fn --attention-split --always-cpu --all-in-fp16 --unet-in-fp8-e4m3fn --disable-server-log --disable-async-cuda-allocation

cd Fooocus && python launch.py --preset anime --vae-in-fp16 --always-offload-from-vram --vae-in-cpu --clip-in-fp8-e4m3fn --attention-split --always-cpu --all-in-fp16 --unet-in-fp8-e4m3fn --disable-server-log --disable-async-cuda-allocation
