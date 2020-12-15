# DeepRL_With_Gym

1,Deep Reinforcement Learning

2,Gym http://gym.openai.com/

Settings:

# Export different directory modules
import sys,os
BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
sys.path.append(BASE_DIR)

# using gpu
config = tf.compat.v1.ConfigProto()
config.gpu_options.per_process_gpu_memory_fraction = 1.0
config.gpu_options.allow_growth = True
tf.compat.v1.Session(config=config)

# using cpu
import os
os.environ["CUDA_VISIBLE_DEVICES"] = "-1"