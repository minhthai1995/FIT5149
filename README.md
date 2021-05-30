# FIT5149
# Introduction 
This work proposed a deep learning model that is capable of detecting the working condition (On - Off) of five appliances, including air conditioner, electric vehicle charger, oven, cloth washer and dryer. 

## Installation
To run the program, some libraries are required.

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install some python packages:

```bash
pip install ...

```
In case you're using Conda or Miniconda, here are sample steps to create an environment (My computer is running Ubuntu OS, core i9, and RTX 3080 GPU, thus you might need some minor changes to get it running on your computer)
```
conda create --name group1ass2 python=3.8.6 pytorch=1.7.1 cudatoolkit=11.0.221 cudatoolkit-dev cmake=3.18.2 cudnn --channel pytorch --channel=conda-forge
conda activate group1ass2
conda install pandas, numpy
conda install -c anaconda scikit-learn, pathlib
conda install -c conda-forge matplotlib, multiprocess, tsfresh, tqdm
```

As Pytorch allow us to train the model using GPU, which is much faster than the current CPU performance. To start, you will need the GPU version of Pytorch, and please make sure that your computer has a higher end NVIDIA GPU that is CUDA enabled, other wise the model will be trained on CPU, we haven't tried to train it on CPU before but pretty sure it will take at least a day.



## Usage
To reproduce the model, the first Jupyter Notebook file that should be run is: "CNN_model_training"
After installing all the required packages, you can simply hit the "Kernel -> Restart and Run All"

The model would take roughly 3 hours to finish the training phase. The final model will be saved in the "trained_model" directory

For the inference and testing part, you can open the "CNN_model_intererence" notebook, and click "Kernel -> Restart and Run All". The output would be generated as a csv file.

## Contribution
If you want to make any contribution to our current work, pull requests are welcome. If you want any further discussion, you can send us an email via: mngu0072@student.monash.edu


