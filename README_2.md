install groundingdino first
    remmberber export CUDA_HOME=/usr/local/cuda12.5 - to the path of cuda first
    conda create -n groundingdino python=3.10
    pip install requirements.txt (from grounding dino repo)
    pip install -e .

then go back to sa3d to 
    pip install requirements.txt  (from sa3d repo)
    sudo apt-get install ninja-build
    pip install mmcv einops 
    also install other necessary dependecise - check the requirements.txt all the version for packeages are correct threre- remmber do not reinstall torch, torch vision there
