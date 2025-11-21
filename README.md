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

2> apt update && apt upgrade -y && apt-get install curl git gcc make build-essential python3 python3-dev python3-pip python3-venv python-is-python3 -y && pip install ffmpeg && apt dist-upgrade -y && apt install wget && apt-get install libgl1 libglib2.0 libsm6 libxrender1 libxext6 -y && apt-get install google-perftools && apt install libgoogle-perftools-dev && pip install moviepy==1.0.3 && pip install accelerate && pip install setuptools && pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu && pip install sageattention && apt-get install git-lfs && pip install diffusers && pip install gguf && pip install numba && pip install pynvml && pip install wheel && pip install docutils && pip install use && pip install numpy._utils && pip install fonttools>=4.22.0 && pip install simpleeval && pip install numexpr && pip && pip install insightface && pip install open-clip-torch && pip install einops && pip install cython && pip install polygraphy && pip install torchsde && pip install wget && apt-get install libavformat-dev libavfilter-dev libavdevice-dev ffmpeg && pip install cmake && apt-get install -y build-essential python3-dev python3-setuptools make cmake && pip install omegaconf && pip install pandas && apt install git-lfs && pip install ip_adapter && pip install accelerator && pip install numpy && pip install gradio && pip install transformers diffusers torch huggingface_hub && pip install exiv2 && pip install music-tag && pip install compel && pip install gfpgan && pip install tomesd && pip install peft && pip install 'controlnet_aux' && pip install 'photomaker' && pip install compiler && pip install torchtext==0.15.2 && pip install soundfile && apt install protobuf-compiler libprotobuf-dev && pip install protobuf && pip install ninja && pip install hpsv2 && apt install python3-tk && apt install qtbase5-dev && pip install mistune && pip install tokenizers==0.21.6 && pip install altair && pip install supervision

4> git clone https://github.com/lllyasviel/Fooocus.git

5> cd Fooocus

'Fix' the issue with Python running in PRoot

export ANDROID_DATA=anything

6> pip install -r requirements_versions.txt


WHEN YOU RESTART TERMUX

./start-ubuntu22.sh

cd Fooocus && python launch.py --preset realistic --always-offload-from-vram --vae-in-cpu --clip-in-fp8-e4m3fn --attention-split --always-cpu --all-in-fp16 --unet-in-fp8-e4m3fn --disable-server-log --disable-async-cuda-allocation

cd Fooocus && python launch.py --preset anime --vae-in-bf16 --always-offload-from-vram --vae-in-cpu --clip-in-fp8-e4m3fn --attention-split --always-cpu --all-in-fp16 --unet-in-fp8-e4m3fn --preview-option taesd --disable-server-log --disable-async-cuda-allocation