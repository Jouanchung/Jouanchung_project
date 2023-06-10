# Jouanchung_project
type: "project" # DON'T TOUCH THIS ! :)
date: "2020-06-09" 
# Decoding working memory load based on EEG signals 

# Your project GitHub repository URL
github_repo: https://github.com/PSY6983-2021/project_template


tags: [EEG, working memory load, machine learning]

# summary

"My project aims to decode WM load based on EEG data. Previous studies have shown that alpha, beta frequency band power are sensitive to working memory processing. I hope to  examine whether the differences in activity patterns of frequencies could be used to decode different WM load."


## Project definition

### Background
Working memory refers to the temporary storage and manipulation of the information. Previous studies have shown that alpha, beta frequency band power are sensitive to working memory processing such as in N-back task. Alpha and Theta power increase with the increasing working memor load. Working memory overload can lead to mental exhaustion and failure in the task. There are only a few studies that decode working memory load from EEG data. Therefore, this study aims to examine whether the differences in the activity patterns of frequency could be used to decode working memory load. 


### Tools

The "project template" project will rely on the following technologies:
 * Markdown, to structure the text.
 * The Hugo website framework which is used by the BHS website. This makes it possible to easily add the markdown project description      to the website.
 * Adding the project to the website relies on github, through pull requests.

### Data
This study adopts Openneuro data ds003838 "EEG, pupillometry, ECG and photoplethysmography, and behavioral data in the digit span task and rest". Only the data that include a sequence of 9 and 13 digits are extracted since the interest of this study lies in the working memory overload.

### Deliverables

At the end of this project, we will have:
 - The current markdown document, completed and revised.
 - Jupyter notebook with code scripts: data preprocessing, machine learning classifiers and data   
   visualization

### Progress overview
This study tried to use EEG data to decode working memory load. The parameter should be changed so that the resolution would be better. That is, I hope to find out the specific frequency that can best decode the working memory load. Moreover, whether the time-frequency in different regions can better decode working memory load. 


### Tools I learned during this project

 * **Python mne package: Decoding in time-frequency space using Common Spatial Patterns (CSP)
 * **Github workflow-** The successful use of this template approach will demonstrate that it is possible to incorporate dozens of students presentation on a website collaboratively over a few weeks.
 * **Project content** Through the project reports generated using the template, it is possible to learn about what exactly the brainhack school students are working on.

## Results
The result shows that the frequency between 7.5-15 within 100-500 milliseconds can be best decoded with accuracy over the chance level. Due to the lack of RAM, I'm now not able to run the code under another parameter. In the future, I might change the parameter to the following parameter.
tmin, tmax = 0, 4.000
n_cycles = 10.0  # 
min_freq = 4.0
max_freq = 25.0
n_freqs = 6  # 

![time-frequency decoding accuracy](https://github.com/Jouanchung/Jouanchung_project/assets/59600450/56c69467-3f1e-47bf-ac52-a3b665981e2e)


The repository of this project can be found [here](http://github.com/Jouanchung/Jouanchung_project). The objective was to create a processing pipeline for EEG data and time-frequency analysis.

