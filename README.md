# mol_finder
Project for finding synthesizable molecules with multiple properties.


## Install Dependencies


#### Install chemprop
    conda create -n chemprop python=3.8
    conda activate chemprop
    conda install pytorch==1.6.0 torchvision==0.7.0 -c pytorch
    conda install -c conda-forge rdkit
    pip install -r requirements.txt
    
#### Install multiobj-rationale
    cd ..
    git clone git@github.com:anonymous20201002/multiobj-rationale.git
    cd multiobj-rationale
    pip install -e .
    cd ../mol_finder
    
## Example to Run
    export CUDA_VISIBLE_DEVICES=0
    export TF_CPP_MIN_LOG_LEVEL=2
    export PYTHONPATH=$PWD
    python mol_finder/main.py --rounds=10 --epoch=1