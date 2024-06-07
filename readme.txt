use jupyter lab this will not work in google colab as there is no display avalaible 
open the whole folder in jupyter lab and run main.ipynb step by step and check the comments  

we tarined the model multiple times and /train/train_basic/best_model_60000 
is the best result that we got 

install all the requirements by execuiting the code cell provided 
please run every code block in sequential order starting from the top with few exceptions such as

 "# this is working for normal devices which does not have gpu enabled etc 
model = PPO('CnnPolicy', env, tensorboard_log=LOG_DIR, verbose=1, learning_rate=0.0001, n_steps=2048)"

and 

"# due to limited time and issues with the gpu we could only run few iterations(it ran for the whole night) but we were able to get good results
# and get a good accuracy
model.learn(total_timesteps=100000, callback=callback)"

as there is no need to train the model again so can be skipped, 
i have mentioned in the comment of the code cells if that cell is not importent

I have provided the details in comment in the main file please refer to them is there is any issue

