## I310D-Assignment-2

## What I'm testing: 
In this analysis, I am testing for the presence of data bias through querying a Perspective API released by Google Jigsaw. I am examining a dataset of internet comments and their scores, and analyzing the toxicity of each comment using both the Perspective API and my own queries. 

## My hypothesis:
Comments containing sexual or sexuality-related terms are more likely to be scored as "toxic" by the Perspective model. Perspective is more biased when scoring comments containing sexual or sexuality-related terms.

## Results:
Through using my own queries and the Perspective API, I was able to extract the comments containing sexual/sexuality-related terms and analyze their toxicity scores given by both the model and manual reviewers. With a threshold of 0.7, it was found that the model over-estimated the number of these toxic comments (with specific terms) compared to manual reviewers. The difference between the number of toxic comments rated by the model and manual reviewers is 78 (918 and 840, respectfully.) These results support my initial hypothesis that the Perspective model is slightly biased towards comments containing sexual/sexuality-related terms. 


## Results decribed more in-depth:
As stated before, my results were that the Perspective was more biased towards comments containing sexual/sexuality-related terms by giving them a higher toxicity score.  I think it's interesting to see how specific terms impact machine learning algorithms that determine how "toxic" a comment is on social media. I theorize that machine learning for these purposes depend heavily on checking to see if a specific term is present in a set of words. I believe the way machine learning works in these circumstances is that it looks for specific words, then also analyzes the words surrounding those terms. 

I wasn't very surprised by my results of the Perspective being more biased towards comments contain sexual/sexuality-related terms because you don't often see people on social media complementing each other with these types of terms. I can't blame the model for over shooting the amount of comments compared to human input because I think with my tested set of terms, there could be some situations where more context is needed to determine whether it's toxic or not. From my understanding of machine learning, it is very hard for an algorithm to determine contextual information.

One thing that I wished I did better however is having a broader set of terms to base my search on. The set of terms I included was based on my prior knowledge, looking at some of the toxic omments, and looking at other websites of sexual/sexuality terms. I know there was an easier way to do it, such as by maybe importing a dataset of these terms into the notebook. That way, a lot mroe terms would be included, resulting in a bigger sample size. I wasn't sure how to do this, so I decided to do it the "harder way." 

# Questions I have:
In what other situations can a Perspective API be used?
How often do data scientists analyze data bias using a Perpective API? 
