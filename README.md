# ReplicationPackage: An Empirical Study of Developer Discussions on Low Code Software Development Challenges (MSR, 20021)

# Link
**MSR, 2021:** https://ieeexplore-ieee-org.ezproxy.lib.ucalgary.ca/document/9463132/

**Presentation:** https://youtu.be/Gf4doZKPXEE


https://user-images.githubusercontent.com/13589148/166091371-46e904f5-37d2-4d88-b561-76aee34f376b.mp4



## MSR21: An Empirical Study of Developer Discussions on Low Code Software Development Challenges

<br>

## Low Code Software Development
Low code software (LCS) development is an emerging paradigm that combines minimal source code with interactive graphical interfaces to promote rapid application development. LCS aims to democratize application development to software practitioners with diverse background. Given that LCS is relatively a new paradigm, it is important to learn about the challenges developers face during their adoption of LCSD platforms. 
From the SO data dump, we extracted all the posts related to these top nine low-code software development platforms. Here is the list of the nine low-code platforms and their associated SO tags:

* Salesforce ('salesforce-lightning', 'lwc', 'lightning', 'salesforce-communities', 'salesforce-chatter', 'salesforce-service-cloud', 'aura-framework).
* Appian ('appian').
* Outsystems ('outsystems')
* AppMaker ('google-app-maker')
* Zoho ('zoho')
* Mendix ('mendix')
* PowerApps ('powerapps', 'powerapps-formula', 'powerapps-selected-items', 'powerapps-collection', 'powerapps-canvas').
* QuickBase ('quickbase')
* Vinyl ('vinyl')


## Benchmark Dataset
We download Stack Overflow June 2020 data dump for this study. Then we extracted low-code related posts based on our tag list. Our tag list was created from the top nine low-code software development platforms. Our data dump included posts from July 2008 to May 2020 and contained around 58,544,636 posts. Out of these posts, 33.4% were questions, 66.6% were answers, and 17.4% questions had accepted answers.



## Codes Folder
In this replication package, we include all the codes that we used in this study. All the codes are inside the Codes and TopicModelling folder. Codes/DataFiltering folder contains the codes that we used for data extraction from SO data dump Posts.xml file. It also includes the Jupyter notebook code that we used to present the graphs, charts, tables. We also included the dataset and codes of our topic modeling inside the Codes/TopicModelling folder.

## Extracted Dataset
This folder contains the posts that we extracted from our June, 2020 SO data dump's 'Post.xml' file. This folder contains three files. Initial_extraction__(low-code_questions_with_negative_score).csv file contains our initial posts extraction file. Later we removed questions with negative scores and the other two files are used as our final extracted dataset with all the questions with non-negative score and their answers. Our final dataset B contained  4,785 posts in total containing 3,597 non-negative scored questions and 1,188 accepted answers. 

## TopicModelling Folder
After the prepossessing, we used Latent Dirichlet Allocation, and the MALLET tool to find out the low-code development related topics that are discussed on SO. The dataset, the Jupyter Notebook code along with our custom stop word list are inside the Codes/TopicModelling folder.


# ManualLabelling Folder
We manually labeled 915 questions and tagged each question a phase based on Agile software development stages. Among these 915 questions, 16 questions (1.7%) were irrelevantly tagged with one of our low-code related tag by the practitioners. 
