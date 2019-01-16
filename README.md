## ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) A sentiment analysis tool using Natural Language Processing on selected Reddit data

### Overview

The other day a friend from class complemented me on handling DSI with calm and composure, and though I took a moment to pause before thanking him, it did make me wonder if I have just been good at feigning it.

In reality my week is a roller-coaster ride which starts off on a high note when I see all the lovely faces in class, a mid-week panic-attack which slings me into a trough, an early morning swim which kicks in a healthy dose of endorphins, before slumping off at the end of the week as I am wrangled away from my happy place.

I would much rather modulate my week so the troughs aren’t so low and the perhaps the peaks not so high. Serendipitously, last week I discovered the happy and sad subreddits — appropriate to temper my mood along the week. It had been working well, but it did get me thinking of how I could extend this modulation to other aspects of my life.

If I am sending off a text, writing a note to my long lost love, or an important email at the end of a tiring day, it would be healthy to have what I have written cross-checked through some sentiment analysis. So, with that in mind, I went about building a natural language processing-based classifier based on the rather rich corpus of verbiage from each of the happy and sad subreddits.

Specifically, I am building a Natural Language Processing-based model which learns from information contained within the 'happy' and 'sad' subreddits, so that when unseen text is entered, it can ascertain whether that text has a happy ot sad sentiment to it. 

> Data science problem: Given some unseen text, classify its sentiment as either 'happy' or 'sad'.

---

### Datasets

I coallated the reddit (subreddit) posts through an existing API, from 2010 onward for each of the 'happy' and 'sad' subreddits, and collected both submission titles and comments. The corpus comprised more than 300,000 observations.

The data was stored in csv files and then read back into a dataframe as input for training the classification algorithm.

Documentation on API used:
psaw: https://github.com/dmarx/psaw
PushshiftAPI: https://github.com/pushshift/api

---

### Deliverables

- A Jupyter notebook, [HB_project-3_reddit.ipynb](./code/HB_project-3_reddit.ipynb), for which a structured format was provided, that describes the data with visualizations and statistical analysis. The final raw data file can be found [here](./data/)
- A README markdown file [this file](./README.md) that provides an introduction to and an overview of the project.
- A presentation [slideshow](./slides/HB_project_3_reddit.pdf) rendered as a .pdf file. The included presentation, intended for a non-technical audience, was presented to the class on December 21st, 2018.

---

### Technical Report and Implementation

I used the [HB_project-3_reddit.ipynb](./code/HB_project-3_reddit.ipynb) Jupyter Notebook to outline the entire process, and is meant to showcase the methodology and implementation for defining the problem, gathering, exploring, and tranforming the dataset, and building, fitting, and evaluating the model to answer the data science question. I have provided commenting and context as much as possible, but in essensce, it is a rather raw working file to provide both methodology and future reference.

In addition, the tail end of the technical report (the Jupyter Notebook file) includes a live textbox which can be used to enter text to be classified.

---

### Executive Summary

Data science problem: Given some unseen text, classify its sentiment as either 'happy' or 'sad'.

Structure
- Inspiration
- Live demo
- Under the hood
- Future improvements
- Insights


Slide-set: [slideshow](./slides/HB_project_3_reddit.pdf)

---
