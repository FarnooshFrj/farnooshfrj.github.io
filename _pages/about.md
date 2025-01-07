---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. student at McGill University, working under the supervision of [Prof. Gregory Dudek](https://scholar.google.ca/citations?user=BSORuFoAAAAJ&hl=en) and [Prof. David Meger](https://scholar.google.ca/citations?user=gFwEytkAAAAJ&hl=en) in the MRL lab. My research journey spans diverse projects, including diver tracking and mapless navigation for off-road RC cars. During my Master's studies, I delved into Artificial Intelligence (AI) for the first time, focusing on driver drowsiness detection.

Over the years, I’ve gained hands-on experience with Vision-Language Models, Transformers, Convolutional Neural Networks, Recurrent Neural Networks, Machine Learning algorithms, and Reinforcement Learning techniques. Currently, my focus is on multi-modal learning for robot in-hand manipulation, with a particular interest in combining vision and tactile data to advance robotic capabilities.

Beyond academics, I strive to live a balanced and fulfilling life. Since January 2022, I’ve embraced self-exploration and mindfulness practices, which have profoundly transformed my perspective. Now in my 30s, I feel like I’m truly living!

I’m not just a researcher—I’m a lifelong learner with a passion for exploring new skills and hobbies. Whether it’s learning French, honing my coding expertise, scuba diving, painting watercolors, or picking up piano, I thrive on creativity and growth.

I stay active with regular workouts and enjoy running during Montreal’s snow-free months. Life is too short to count candles on a cake, so I focus on cherishing every moment.


Recent Publications
------
This section features my most recent publications, accompanied by their abstracts. You can explore project videos in the Demo section for a closer look at each project.

**[Uncertainty-aware hybrid paradigm of nonlinear MPC and model-based RL for offroad navigation: Exploration of transformers in the predictive model](https://ieeexplore.ieee.org/abstract/document/10610452)**

In this paper, we investigate a hybrid scheme that combines nonlinear model predictive control (MPC) and model-based reinforcement learning (RL) for navigation planning of an autonomous model car across offroad, unstructured terrains without relying on predefined maps. Our innovative approach takes inspiration from BADGR, an LSTM-based network that primarily concentrates on environment modeling, but distinguishes itself by substituting LSTM modules with transformers to greatly elevate the performance of our model. Addressing uncertainty within the system, we train an ensemble of predictive models and estimate the mutual information between model weights and outputs, facilitating dynamic horizon planning through the introduction of variable speeds. Further enhancing our methodology, we incorporate a nonlinear MPC controller that accounts for the intricacies of the vehicle’s model and states.

**[Constrained Robotic Navigation on Preferred Terrains Using LLMs and Speech Instruction: Exploiting the Power of Adverbs](https://link.springer.com/chapter/10.1007/978-3-031-63596-0_11)**

This paper explores leveraging large language models for mapless offroad navigation using generative AI, thereby eliminating the need for data collection and annotation. We propose a method where the robot receives speech instructions, converted to text through Whisper, and a large language model (LLM) like GPT model extracts landmarks, preferred terrains, and crucial adverbs translated into speed settings for constrained navigation. A language-driven semantic segmentation model generates text-based masks for identifying the required landmarks and terrains in images. By translating 2D image points to the vehicle’s motion plane using camera parameters, an MPC controller guides the vehicle towards the desired terrains. This approach enables adaptability to diverse environments and enhances instructions for navigating complex and challenging terrains.

**[Drowsiness detection based on driver temporal behavior using a new developed dataset](https://arxiv.org/abs/2104.00125)**

Driver drowsiness detection has been the subject of many researches in the past few decades and various methods have been developed to detect it. In this study, as an image-based approach with adequate accuracy, along with the expedite process, we applied YOLOv3 (You Look Only Once-version3) CNN (Convolutional Neural Network) for extracting facial features automatically. Then, LSTM (Long-Short Term Memory) neural network is employed to learn driver temporal behaviors including yawning and blinking time period as well as sequence classification. To train YOLOv3, we utilized our collected dataset alongside the transfer learning method. Moreover, the dataset for the LSTM training process is produced by the mentioned CNN and is formatted as a two-dimensional sequence comprised of eye blinking and yawning time durations. The developed dataset considers both disturbances such as illumination and drivers' head posture. To have real-time experiments a multi-thread framework is developed to run both CNN and LSTM in parallel. Finally, results indicate the hybrid of CNN and LSTM ability in drowsiness detection and the effectiveness of the proposed method.

