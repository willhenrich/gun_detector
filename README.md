# gun_detector

### A Nerf Gun in Boston

Last week, a school in Boston went into lockdown because of a report of a student with a gun. Police found that [it was in fact a Nerf toy gun](https://www.nbcboston.com/news/local/nerf-gun-prompts-police-response-to-boston-latin-academy/3245333/). Had it been caught on camera by ZeroEyes, this might have been prevented. To this end, I've created a simple gun detector model, which accurately classifies images of real guns vs. toy guns and hands that aren't holding guns at all. It achieves perfect recall and precision on a 54-image validation set with less than ten epochs of training.

### The Model

The code below shows how I created the model using the the fast.ai library. I created a dataset of 272 images from DuckDuckGo search and cleaned them manually. Then I used the dataset to fine-tune several image classification models. Throughout, I use ideas and code from the [fast.ai course](https://course.fast.ai/) and feedback from ChatGPT. The code can be reviewed and tested as a [Jupyter notebook](https://github.com/willhenrich/gun_detector/blob/main/Henrich_Gun_Detector.ipynb), and the cleaned data is available at in the "hands" directory [here](https://github.com/willhenrich/gun_detector/tree/main).

<br>

![image](https://github.com/willhenrich/gun_detector/assets/84203568/da036dbc-06dc-4cf5-b663-0b0c9ad0f354)
