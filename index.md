## Welcome to the VU course Applied Machine Learning

This course is aimed at PhD students of the VU, who wish to integrate state-of-the-art machine learning techniques in their research. Perhaps you have come across  web-scraping, efficient training of algorithms or computer vision, but do not fully know yet how you can take advantage of these techniques yourself. In this course, we will take you by hand and explore the potential together. We will take a hands-on approach and provide elementary code, which you can easily adapt and extend for your own purposes. We will use the R programming language, and all code will be annotated, sorted per topic and clearly illustrated in biteable chunks. Next, we will host two guest lectures, each providing an example of how to exploit machine learning relevant to topics in the M&O discipline. 

* * *

### Course Schedule

| Week        | Topics                                        | Speakers                       |
|:------------|:----------------------------------------------|:-------------------------------|
| 1           | Introduction + Coduction cycle                | Prof. Dr. A. van Witteloostuijn & Paul Stroet |
| 2           | Natural Language Processing: Automated Literature Reviews | Prof. Dr. S. Khapova & Paul Stroet |
| 3           | Supervised Learning + Data Imputation         | Dr. B. Bosma & Paul Stroet                  |
| 4           | Machine Learning in OB                        | Dr. J. Oostrom & Paul Stroet                |
| 5           | Longitudinal data: Case study                 | Dr. J. Brassey & Paul Stroet   |
| 6           | Unsupervised learning + Web-scraping          | Paul Stroet                    |

* * *

### Week 1: Introduction + Natural Language Processing

In the first week, we cover the following topics: 

- String basics
- Sentiment analysis
- Topic modeling
  - Latent Dirichlet Allocation
  - Non-negative Matrix Factorization

#### Code

In the programming language R, text data is internally stored as `character` type. The code below illustrates how you can work with this. 

```R
// R code.

# String basics
string <- c("Welcome to the Applied Machine Learning course")
nchar(string) # 46 characters

library(stringi)
str_locate(string, "Applied") # locate first occurrence of the word "Applied"
str_locate_all(string, "a") # locate all occurrences of "a", note the case sensitivity
```

Sentiment encapsulates an opinion of a person (1), about a target or aspect of the target (2), that has a certain valence (+/-/0) or emotion (3) and strength (4). Quantifying sentiment in the simplest sense is done by just counting the number of negative and positive words, and making up the balance. The example below operationalizes this idea.

```R
# Sentiment analysis basics
string <- c("I love Amsterdam with its beautiful canals, fabulous restaurants and terrific history, although there is quite some outdoor noise late at night. The sport facilities the city offers are not bad at all.")
# count positive words: "love, beautiful, fabulous, terrific" -> 4
# count negative words: "noise, bad" -> 2
# count balance of valence words: 4 - 2 = 2 -> in general this string is positive

# Is bad really negative here? In other words, are there ways to account for negations and amplifiers?
```

Now, instead of manually counting the valence words, we can rely on sentiment and emotion dictionaries, in which lists of valence loaded words are collected. 

#### Knowledge clip
Please find the knowledge clip for the first week here (link will follow), in which the importance of cleaning text data (stemming, removing stop-words, etc.) is addressed, and how to do this in an automated and fast fashion. 

* * *

### Week 2: Web-scraping

Coming soon

* * *

### Support or Contact

Having trouble setting up the right configurations in R, or installing the correct packages? Check out our documentation (link will follow) in which the configurations of my R version are outlined, or send an e-mail to p.stroet@businessdatascience.nl and we’ll help you sort it out. 

### Thoughts

NLP, split in multiple lectures. One with the basics, second with sentiment analysis, third with topic modeling, fourth with predictive modeling.

Additional topics: Deep Learning, covering neural nets; Network Analysis, extracting nodes and using them in a predictive model.

Or, cover basics in this course (AML I), and dive into more depth tailored to the global needs in eg AML II.

First offered as summer school, then in a block in the academic year, and then scale it up to a MOOC

8 weeks of interesting lectures, concluded with an assignment in which you accelerate a current project by adopting one of the techniques taught in this course
you also need to present your paper, and you will give your peers feedback on the presentation
