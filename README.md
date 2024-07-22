Holy $%!+ This Works on 12gb Ram!!!

# FOOOCUS_ANDROID_TERMUX

The New 2.5.0 Update Works On 12gb Ram Cpu Mode
I had to use developer advanced settings to use this u can use sd1.5 and sdxl also change refiner to vae mode and I used miniSD.ckpt
it's trained on 256x256 images plus I used ssd-1b distilled sdxl for more memory saved.
now I can use fooocus officially on my phone!
Also go into developer options and enable skip preprocessor that will also save memory yes the advanced tab developer options is your friend don't use the presets like speed quality etc.... enable developer and overide the width and height of your image to at least for me 320x512 for sdxl. if u override refiner you can put it at 0 idk if that made it switch instantly or cause when I did it it switched on last step maybe cause I used vae refiner mode but enjoy and I changed the command args for more memory saved.;)




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


here is a prepaid fooocus preset I haven't tested it yet but you can try it out if you want?

https://github.com/KintCark/FOOOCUS_ANDROID_TERMUX/blob/main/Cpu%20Android%2012gb%20Ram.json