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

### Week 1: Introduction + Natural Language Processing

#### Code

```R
// R code.

# String basics
string <- c("Welcome to the Applied Machine Learning course")
nchar(string) # 46 characters
str_locate(string, "Applied") # locate whole words
str_locate_all(string, "a") # locate single letters, note the case sensitivity
```

#### Knowledge clip
Please find the knowledge clip for the first week here (link will follow). 

* * *

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
