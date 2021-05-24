## Welcome to the VU course Applied Machine Learning

This course is aimed at PhD students of the M&O department, who wish to integrate state-of-the-art machine learning techniques in their research. Perhaps you have come across  web-scraping, efficient training of algorithms or computer vision, but do not fully know yet how you can take advantage of these techniques yourself. In this course, we will take you by hand and explore the potential together. We will take a hands-on approach and provide elementary code, which you can easily adapt and extend for your own purposes. We will use the R programming language, and all code will be annotated, sorted per topic and can be find below. Next, we will host two guest lectures, each provides an example of how to exploit machine learning relevant to the M&O discipline. 

### Course Schedule

| Week        | Menu                                          | Speakers                       |
|:------------|:----------------------------------------------|:-------------------------------|
| 1           | Introduction + Natural Language Processing    | Prof. S. Khapova & Paul Stroet |
| 2           | Web-scraping                                  | Paul Stroet                    |
| 3           | Supervised learning                           | Paul Stroet                    |
| 4           | Unsupervised learning                         | Paul Stroet                    |
| 5           | Guest Lecture: Automated Literature Reviews   | Prof. S. Khapova               |
| 6           | Guest Lecture: Interpretable Machine Learning | Prof. A. van Witteloostuijn    |

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
# Sentiment Analysis
string <- c("I love Amsterdam with its beautiful canals, fabulous restaurants and terrific history, although there is quite some outdoor noise late at night. The sports facilities the city offers are not bad at all.")
# count positive words: "love, beautiful, fabulous, terrific" -> 4
# count negative words: "noise, bad" -> 2
# balance of valence words: 2

# Q: is bad really negative here? 
```

#### Knowledge clip
Please find the knowledge clip for the first week here (link will follow), in which the importance of cleaning text data (stemming, removing stop-words, etc.) is addressed. 

* * *

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

### Thoughts

NLP, split in multiple lectures. One with the basics, second with sentiment analysis, third with topic modeling, fourth with predictive modeling
Additional topic: Deep Learning, covering neural nets
