# Decision_Transformer-for-Minari-dataset
Decision Transformer in PyTorch for mujoco Pointmaze in OpenAI gymnasium. 

# Overview
This repository is mainly based on the [min-decision-transformer](https://github.com/nikhilbarhate99/min-decision-transformer). 
#### The key differences from min-decision-transformer and [official decision transformer](https://github.com/kzl/decision-transformer) are: 
  - Replacing the outdated gym with new [OpenAI gymnasium](https://gymnasium.farama.org/content/basic_usage/)
  - Implementing the decision transformer for continuously controlling the ball in Pointmaze environment. (More environments will be avaliable)
  - A jupyter notebook is provided to show beginners how to download the Minari dataset and the data types within it.

# Results
  Example of running detials | record 
  ------------- | -------------
  num of updates:| 20000 |  
  action loss:| 0.14227
  eval avg reward:| 0.75000
  eval avg ep len:| 382.50000
  eval d4rl score:| 80.00000
  max d4rl score:| 94.00000
  ![](https://github.com/WangJinCheng1998/Decision_Transformer-for-Minari-dataset/blob/main/pointmaze.gif)  | ![](https://github.com/WangJinCheng1998/Decision_Transformer-for-Minari-dataset/blob/main/pointmaze2.gif)       

# Steps
## Install gymnasium 0.29.1

     pip install gymnasium==0.29.01

## Install Mujoco

English: [GO this link](https://github.com/openai/mujoco-py)

Chinese:  Following the steps in this [BLOG](https://blog.csdn.net/weixin_44612539/article/details/127555145) :step2 -step 5  


## Install Minari dataset

    pip install minari
    
  ### Downloading Pointmaze_umaze dataset

    import minari
    minari.download_dataset(dataset_id="pointmaze-umaze-v1")

  ### Jupyter notebook for beginners to understand the data type inside the dataset


   - [ ] :smiley: [Simple_gymnasium](https://github.com/WangJinCheng1998/Decision_Transformer-for-Minari-dataset/blob/main/Simple_gymnasium.ipynb)



# References
Basic model:[Min Decision_transformer](https://github.com/nikhilbarhate99/min-decision-transformer),[official decision transformer](https://github.com/kzl/decision-transformer).

For the offline learning dataset:[Minari](https://minari.farama.org/main/content/basic_usage/)
