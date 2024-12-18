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

I’m not just a researcher—I’m a lifelong learner and a passionate explorer of hobbies. I’m learning French, improving my coding skills, painting with watercolors, and recently began playing the piano. I work out regularly, run three days a week in spring and summer (avoiding Montreal's icy winters!), and most importantly, I’ve stopped counting the candles on the cake. Instead, I savor every moment.


A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, Academic Pages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over - just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this template](https://github.com/academicpages/academicpages.github.io) by clicking the "Use this template" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Recent Publications
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Uncertainty-aware hybrid paradigm of nonlinear MPC and model-based RL for offroad navigation: Exploration of transformers in the predictive model**

n this paper, we investigate a hybrid scheme that combines nonlinear model predictive control (MPC) and model-based reinforcement learning (RL) for navigation planning of an autonomous model car across offroad, unstructured terrains without relying on predefined maps. Our innovative approach takes inspiration from BADGR, an LSTM-based network that primarily concentrates on environment modeling, but distinguishes itself by substituting LSTM modules with transformers to greatly elevate the performance of our model. Addressing uncertainty within the system, we train an ensemble of predictive models and estimate the mutual information between model weights and outputs, facilitating dynamic horizon planning through the introduction of variable speeds. Further enhancing our methodology, we incorporate a nonlinear MPC controller that accounts for the intricacies of the vehicle’s model and states.

**Constrained Robotic Navigation on Preferred Terrains Using LLMs and Speech Instruction: Exploiting the Power of Adverbs**

This paper explores leveraging large language models for mapless offroad navigation using generative AI, thereby eliminating the need for data collection and annotation. We propose a method where the robot receives speech instructions, converted to text through Whisper, and a large language model (LLM) like GPT model extracts landmarks, preferred terrains, and crucial adverbs translated into speed settings for constrained navigation. A language-driven semantic segmentation model generates text-based masks for identifying the required landmarks and terrains in images. By translating 2D image points to the vehicle’s motion plane using camera parameters, an MPC controller guides the vehicle towards the desired terrains. This approach enables adaptability to diverse environments and enhances instructions for navigating complex and challenging terrains.

**Drowsiness detection based on driver temporal behavior using a new developed dataset**

Driver drowsiness detection has been the subject of many researches in the past few decades and various methods have been developed to detect it. In this study, as an image-based approach with adequate accuracy, along with the expedite process, we applied YOLOv3 (You Look Only Once-version3) CNN (Convolutional Neural Network) for extracting facial features automatically. Then, LSTM (Long-Short Term Memory) neural network is employed to learn driver temporal behaviors including yawning and blinking time period as well as sequence classification. To train YOLOv3, we utilized our collected dataset alongside the transfer learning method. Moreover, the dataset for the LSTM training process is produced by the mentioned CNN and is formatted as a two-dimensional sequence comprised of eye blinking and yawning time durations. The developed dataset considers both disturbances such as illumination and drivers' head posture. To have real-time experiments a multi-thread framework is developed to run both CNN and LSTM in parallel. Finally, results indicate the hybrid of CNN and LSTM ability in drowsiness detection and the effectiveness of the proposed method.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
