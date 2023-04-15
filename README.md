# Image-Analysis-Election-Prediction-Project
This is a repository of my **machine learing project** that uses facial images of political candidates to predict their success. This repository includes non-finalized versions of the machine learning program and the dataset that I used.

Link to my **dataset**, file size was too big for Github (https://www.kaggle.com/datasets/raymonddeminglin/us-and-cn-candidates-facial-images-2000-present)

**Information about my project (A Novel Approach to Detecting Unconsciousness in Human Decision-Making using Machine Learning):**


**-----Inspiration---------------**

Although much is known about the conscious and subconscious parts of your brain, more research is still needed on the inner workings of the unconscious mind. Unlike how it is defined in Freudian psychoanalysis, unconscious thought is referred to in this project as mental processes that are outside the realm of consciousness or awareness but influence judgments, feelings, or behavior. We use unconscious thought, brain, and mind as synonymous terms.

The exact influence that your unconscious mind has on your decision making and perception of the world is a subject of much debate: whereas some believed that the unconscious mind governs a significant amount of your behaviour, others believe that the majority of it is kept “locked up” in the deep recesses of your brain without affecting any of your real-world actions. Understanding the unconscious mind is crucial to many aspects of science now and in the future: the advancement of cognitive science, of sociology, of behavioral economics, and artificial intelligence. The purpose of our project is to use technology to establish the extent of influence that the unconscious mind has on conscious decision making. Specifically, we were inspired to explore cognitive science due to the alarming rise of mental illnesses and alcohol/drug abuse—especially among youth—during modern times as technology develops and professional industries become more competitive. Since the unconscious mind is where many scientists believe lies the source of repressed or traumatic emotions, further research of that area of the brain could lead to new and innovative ways to treat mental illnesses.

We chose to conduct this investigation by using elections as a case study of an important decision presumably made using conscious thought and analysis. The vast majority of voters weigh the actual qualifications, track record, beliefs, and competence of politicians before voting, and we assume that they do not consciously base their decisions on the facial attractiveness or features of a candidate. As such, we wish to make a machine learning model which can process candidates based only on a picture of their face and predict their success within an election. If we are able to make a model which is more than 50% accurate in predicting election outcomes given only a picture of a candidate's face, it would be a demonstration of the impact that your unconscious mind has on your conscious decision making. Since voters don’t consciously base their decisions on the facial features of a politician, the only other explanation of the results would be that your unconscious judgements based on appearance played a part in your actual decision making, without even being aware of this unconscious thinking.


**-----Introduction---------------**

Similar to our project, researchers have tried to explore human decision by building machine learning models to predict election outcomes from images of faces (Joo et al., 2015; Todorov et al., 2005; Ventura et al., n.d.). Many of these models have near-human accuracy. For example, an extensive machine learning study (Joo et al., 2015) was able to reach a 67.9% accuracy in predicting the US governor races. They gathered a dataset of 650 senators and extracted values of their facial traits before collecting some of the values via human input to give relative rankings, and collected other values via digital facial segmentation. They then combined these data as input for a multi class SVM.

Despite the impressive accuracy of this study, we believe that more work is needed in the industry to fully explore this problem—our project seeks to build upon and improve these previous such studies to fully explore cognitive science. For example, in the example mentioned above (Joo et al., 2015) the researchers themselves named the categories of attributes that they want to extract, which could lead to certain physical features left ignored or under-represented. Furthermore, a significant portion of the input data used for the training came from human participants to begin with; the model likely would not have achieved such a high accuracy without human contribution. In summary, previous methods such as those used in (Joo et al., 2015) relied on assumptions that introduced biases into how the algorithm made its prediction. In order to have a truly unbiased machine learning model, we directly input the image of the politician without specifically extracted traits or human input.

Overall, while there have been many past studies that try to predict election results through machine learning—as outlined above—it is important to note that very few of them account for human irrationality and rather, look at things such as economic status, political ideology, etc. We attempt to set our project apart from other similar studies by basing our predictions solely off of physical features to predict the outcome of an election and establish the influence of unconsciousness within voter decision making rather than looking at the more obvious factors that play into your conscious decisions, such as political stance and policies.

With regards to the methodology, we sought to train a machine learning model to predict the outcome of an election from a facial image of a candidate. As far as we know, previous studies on this subject all paired politicians during their experimental or data collection process, training the model to predict which of the two candidates will win the election. This pairing was often either derived from the two candidates running against each other (Ballew & Todorov, 2007), or the two candidates with a similar perceived age (Joo et al., 2015). This might make sense at first glance, as one would think that to evaluate the competence of a politician, there has to be a relative comparison. However, our experiment uniquely challenges that preconception by not using any sort of pairing in the process. All the data we used were individually selected from an array and individually evaluated, with “winner” or “loser” as the only label. This allowed us to dramatically reduce the amount of data needed to train the model due to the quadratic nature of pairwise predictions. Furthermore, this leads to more versatile and applicable results in the case of re-election or scenarios where more than two candidates are frontrunners. We can also prevent issues resulting from pairing and assess each candidate individually to provide more accurate results, since we can establish the probability of a candidate winning in any situation—not just against a specific opponent.
