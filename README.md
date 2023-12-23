# How to Run Spot Micro Simulation in Pybullet
In this tutorial, I will show you how to run the Spot Micro simulation with pybullet using python in VS Code. I will go through step by step from installing python, cloning the repo, installing all the necessary modules and the exact commands to run the simulation using the env_tester.py file. I will go over the different simulation modes for Spot Micro by using different command line arguments. Finally, I will go over the env_tester.py file and briefly discuss the structure of the code and the modules used in this simulation. 

Click Img Below to See Youtube Video:
[![](https://img.youtube.com/vi/kSqqniOEf6Q/0.jpg)](https://youtu.be/kSqqniOEf6Q)

## Spot Micro Overview
https://spotmicroai.readthedocs.io/en/


## Installing Python
Install `python 3.8.10`
https://www.python.org/downloads/release/python-381/

## Clone spot_mini_mini Repo
```bash
git clone https://github.com/OpenQuadruped/spot_mini_mini.git
```

## Setup Virtual Environment
Create and activate virtual environment. Add my `requirements.txt` file to the `spot_mini_mini` repo.
```bash
py -3.8 -m venv env3_8
.\env3_8\Scripts\activate
pip install -r .\requirements.txt
```

## Run Spot Micro in Basic Mode
```bash
cd .\spot_bullet\src\ 
python .\env_tester.py
```

## Run Spot Micro with Foot Path 
```bash
python .\env_tester.py -p
```

## Run Spot Micro on Elevated Rack
```bash
python .\env_tester.py -r
```

## Run Spot Micro with Reset Mode (When Spot Gets Stuck)
```bash
python .\env_tester.py -ar
```

## Review Spot Micro Pybullet Simulation Code
Review `env_tester.py` file. 