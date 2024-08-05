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

    pip install imageio[ffmpeg] imageio[pyav]
    pip install --upgrade transformers flask dash

python run.py --config=configs/llff/fern.py --stop_at=20000 --render_video --i_weights=10000

python run_seg_gui.py --config=configs/llff/seg/seg_fern.py --segment --sp_name=_gui --num_prompts=20 --render_opt=train --save_ckpt


add os.environ['QT_QPA_PLATFORM'] = 'offscreen' to the main() so that we can debug the code