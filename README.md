# Project Title

DSC160 Data Science and the Arts - Final Project - Generative Arts - Spring 2020

Project Team Members: 
- Mariam Qader, maqader@ucsd.edu
- Molly Rowland, mhrowlan@ucsd.edu
- Myra Haider, myhaider@ucsd.edu
- Enrique Sanchez, ens004@ucsd.edu
- Alexandria Kim, aek005@ucsd.edu

## Abstract

For our generative art project, we are interested in the condition synesthesia. This is the condition where a person’s senses are mixed, such as tasting color, or hearing textures. It affects “at least 4% of the population” of the US and there are more than 50 forms of synesthesia(Wu). One way to help others understand this condition, is by using generative art methods to create synthetic synesthesia for those who don’t have the condition. 
We plan to make a neural network to transform text and sound to color. Many of the articles we found on this subject discuss using GAN to create the deep learning model. One of the papers discusses taking a database of handwritten characters, implemented as a multilayer convolutional neural network, and having a separate multilayer convolutional neural network to create a colored version of the text based on a grapheme-color synesthetes(Bock). We also found an example of someone taking an audio file and creating images of landscapes and humans (Laken). From these two examples, we hope to combine them to create our own responsive model. In order to convert sound to color, we can use the frequency of a note to generate a hexadecimal or RGB value. An important observation to note is that the mapping of a sound to color varies amongst individuals, so we will attempt to create a model that arbitrarily generates this mapping. Spectrograms are an example we have seen in class of audio being represented visually. We’d like to build upon this idea by focusing on notes instead of just waveforms, as well as using the relationship between color and sound to replicate synesthesia. AudioPaint by Nicolas Fournel is a similar example that converts images to sound, translating attributes such as brightness and pixel position to volume and frequency. 
Our current plan is to arbitrarily assign each letter to a note and color. From this, when a word is entered, we will return some pattern of notes and colors. The user can input a word of their choice, and our model will output an image containing the colors associated with the letters in the word (e.g. https://synesthesia.me/see-your-name). Additionally, we would like to incorporate sound into our project by having a song played as well. Each letter will be associated with a single note. Our model will play a mini phrase of the combination of notes according to the word the user input. Therefore, the output will be both visual and vocal. Our goal is to make an interactive widget through Python libraries like Holoviz that will produce a jpg image of colors and a .wav sound file based on the user inputed text. Some challenges that may arise while working on this project include finding enough images that contain the colors associated with the words inputted. We may have to create some parameters as to what words are acceptable to input (i.e. maximum length of 10 letters). Through our project we hope to take both the technical and qualitative skills we have been shown in class and apply them to our area of interest. We will be using GAN to implement our project to help us gain a greater understanding of synthesia and how it affects the people around us. Many of the example projects shown in class help us understand different people and cultures through technology, which is exactly what we hope to achieve here. Synesthesia is an interesting condition to study as it provides insight into how the brain perceives things. It gives us a chance to see how people with this condition perceive the world, and helps us understand how the world can look very different to everyone. This project will also allow us to learn more about the condition, and the effects it has on different people. 
List three papers / art projects that are references for this work.
https://towardsdatascience.com/synesthesia-an-inspiring-condition-for-ai-researchers-10cd57708855
https://www.mdpi.com/2504-2289/2/1/8/pdf 
https://synesthesia.me/see-your-name
https://www.medicalnewstoday.com/articles/322807#Mechanisms-and-causes
https://www.livescience.com/60707-what-is-synesthesia.html
https://panel.holoviz.org/
https://paulvanderlaken.com/2019/10/29/neural-synthesia-gan-ai-dreaming-of-music/
https://designingsound.org/2017/12/20/mapping-sound-to-color/
http://www.nicolasfournel.com/?page_id=125#comment-4827





Works Cited
Bock, Joel R. “A Deep Learning Model of Perception in Color-Letter Synesthesia.” 2017, doi:10.20944/preprints201712.0128.v1.
Laken, Paul van der. “Neural Synesthesia: GAN AI Dreaming of Music.” Paulvanderlaken.com, 30 Oct. 2019, paulvanderlaken.com/2019/10/29/neural-synthesia-gan-ai-dreaming-of-music/.
“Type Your Name.” What Color Is Your Name?, synesthesia.me/see-your-name.
Wu, Jun. “Synesthesia, An Inspiring Condition For AI Researchers.” Medium, Towards Data Science, 27 Jan. 2020, towardsdatascience.com/synesthesia-an-inspiring-condition-for-ai-researchers-10cd57708855.
## Data and Model

(10 points) 

In the final submission, this section will describe both the data you use for this project and any pre-existing models/neural nets. For each you should provide the name, a textual description, and a link. If there is a paper (for neural net) link that as well.
- Such and such Neural Net. The short description of this neural net. 
  - [link to code]().
  - [Title of Paper with Link](). 
- Training data. Short description of training data including bibliographic info. [link to data]().

## Code

(20 points)

This section will link to the various code for your project (stored within this repository). Your code should be executable on datahub, should we choose to replicate your result. This includes code for: 

- code for data acquisition/scraping
- code for preprocessing
- training code (if appropriate)
- generative methods

Link each of these items to your .ipynb or .py files within this seection, and provide a brief explanation of what the code does. Reading this section we should have a sense of how to run your code.

## Results

(30 points) 

This section should summarize your results and will embed links to documentation to significant outputs. This should document both process and show artistic results. This can include figures, sound files, videos, bitmaps, as appropriate to your generative art idea. Each result should include a brief textual description, and all should be listed below: 

- image files (`.jpg`, `.png` or whatever else is appropriate)
- audio files (`.wav`, `.mp3`)
- written text as `.pdf`

## Discussion

(30 points, three to five paragraphs)

The first paragraph should be a short summary describing your results.

The subsequent paragraphs could address questions including:
- Why is this culturally innovative?
- How does your generative computational approach differ from traditional art/music/cultural production? 
- How do your results relate to broader social, cultural, economic political, etc., issues? 
- What are the ethical concerns for this form of generative art? 
- In what future directions could you expand this work?

## Team Roles

Provide an account of individual members and their efforts/contributions to the specific tasks you accomplished.

## Technical Notes and Dependencies

Any implementation details or notes we need to repeat your work. 
- Additional libraries you are using for this project
- Does this code require other pip packages, software, etc?
- Does this code need to run on some other (non-datahub) platform? (CoLab, etc.)

## Reference

All references to papers, techniques, previous work, repositories you used should be collected at the bottom:
- Papers
- Repositories
- Blog posts
