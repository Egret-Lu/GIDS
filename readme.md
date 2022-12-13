---
editor_options: 
  markdown: 
    wrap: 72
---

<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->

<a name="readme-top"></a> <!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->

<!-- PROJECT SHIELDS -->

```{=html}
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-20



<!-- PROJECT LOGO -->
```
<br />

::: {align="center"}
<a href="https://github.com/github_username/repo_name">
<img src="images/gids.jpeg" alt="Logo" width="280" height="80"/> </a>

<h3 align="center">

GIDS:Understanding Masters' Applicant Pool

</h3>
:::

<!-- TABLE OF CONTENTS -->

<details>

<summary>Contents</summary>

<ol>

<li>

<a href="#about-the-project">Abstract</a>

<ul>

<li><a href="#built-with">Built With</a></li>

</ul>

</li>

<li>

<a href="#getting-started">Getting Started</a>

<ul>

<li><a href="#prerequisites">Prerequisites</a></li>

<li><a href="#installation">Installation</a></li>

</ul>

</li>

<li><a href="#usage">Usage</a></li>

<li><a href="#figure-list">Figure List</a></li>

<li><a href="#code-outline">Code Outline</a></li>

<li><a href="#roadmap">Roadmap</a></li>

<li><a href="#contact">Contact</a></li>

<li><a href="#acknowledgments">Acknowledgments</a></li>

</ol>

</details>

<!-- ABOUT THE PROJECT -->

## Abstract

::: {align="center"}
<a href="https://github.com/github_username/repo_name">
<img src="images/gids2.jpg" width="280" height="200"/> </a>
:::

Sponsor: [GIDS](https://www.sas.rochester.edu/dsc/)

Project Link: [GIDS github](https://github.com/Egret-Lu/GIDS)

This report presents our analysis of selection criteria and application
procedure for graduate school admission across three programs from the
Arts, Sciences, and Engineering (AS&E) program at the University of
Rochester, including Computer Science, Data Science, and Electronic
Chemical Engineering. Specifically, it unfolds applicants' characters in
three ways: applicants' demographic information, applicants' behavior,
and applicants' decision. It begins with an overview of the dataset,
followed by exploratory data analysis results, and concludes with
predictive models. Techniques to handle missing values that are not
completely at random and algorithms to overcome data imbalance are
explored. Implications and limitations are also discussed in this
report.

Codes of the project is mainly based on python programming.

<p align="right">

(<a href="#readme-top">back to top</a>)

</p>

### Built With

-   pandas

-   numpy

-   matplotlib

-   seaborn

-   nltk

-   sklearn

    <p align="right">

    (<a href="#readme-top">back to top</a>)

    </p>

<!-- GETTING STARTED -->

## Getting Started

This is an example of how you may give instructions on setting up your
project locally. To get a local copy up and running follow these simple
example steps.

<!-- Install modules -->

### Installation

Install required modules in terminal `pip install -r requirements.txt`

<p align="right">

(<a href="#readme-top">back to top</a>)

</p>

<!-- USAGE EXAMPLES -->

## Usage

1.  Data File: unzip DATA.zip
2.  User Profile Analysis: EDA_applicant_profile.ipynb
3.  User Behavior Analysis: EDA_applicant_behaviour.ipynb
4.  Prediction Model: Classification_models.ipynb

For more explanations, please refer to the
[Report](https://www.overleaf.com/read/bqbxfrycbmhf)

<p align="right">

(<a href="#readme-top">back to top</a>)

</p>

<!-- Figure -->

## Figure List

Figures shows in the
[report](https://www.overleaf.com/read/bqbxfrycbmhf)

1.  EDA_applicant_profile.ipynb： Fig 1, 2, 3, 4, 5, 6, 7, 25, 27
2.  EDA_applicant_behaviour.ipynb： Fig 8, 9, 10, 11, 12, 13, 14, 26
3.  Classification_models.ipynb： Fig 19,20,21, 22, 23, 24

<p align="right">

(<a href="#readme-top">back to top</a>)

</p>

<!-- outline -->

## Code Outline

Here is the outline of all our codes

### EDA

1.  EDA_applicant_profile.ipynb：

    -   Who applies to each of our programs?
    -   What is the makeup of those who get admitted and those who
        accept our offer.
    -   Using application data, analyze master forn different programs
    -   Compare the data of admitted, rejected, accepted or denied
        students.
    -   Common info age, M/F, URM, international, GPA, TOEFL/IETLS, GRE
    -   Trends of the applicants

2.  EDA_applicant_behaviour.ipynb：

    -   Derive insights on the application timeline
    -   Understand the types of institutions/programs people are
        choosing to attend.

### Model

Classification_models.ipynb:

1. Data Preprocessing:
  - Missing Data Handling: 
    - Deletion: Missing >10% 
    - Imputation: fill with 01
  - Feature Engineering:
    - Focus on features that unsubmitted ones did not fill in such as grade, job, institution and reference
    - Generate new variables based on existed ones (e.g. number of previous jobs, completed references, previous institutions and other applied colleges)       -Data Transformation:
    -Categorical variables: Transform to one-hot encoder (dummy variables)
    - Normalization: MinMaxScaler      

2.  Predict which students will submit/un submit our offer of admissions?

  - Gaussian Mixture
  - SMOTE+ Linear SVM
3.  Predict which students will accept/decline our offer of admissions?
  - SVM (polynomial of degree 2) 
  - SVM (RBF kernel)
  - Gaussian Naive Bayes
  - Gaussian Process
  - K Nearest Neighbour
  - Quadratic Discriminant Analysis


<!-- ROADMAP -->

## Roadmap

-   [ ] 2022-9-28: Project Charter
-   [ ] 2022-10-17: Goal 1 & Goal 3 Merging Datasets
-   [ ] 2022-10-26: Goal 2 EDA
-   [ ] 2022-11-2:[Mid-Term
    Presentation](https://docs.google.com/presentation/d/1Yqd0spkCZES3Iia8LSHgBdiUbmiSxVwrGWw0FAfmaII/edit?usp=sharing)
-   [ ] 2022-11-16: EDA Goal 2 Prediction & Goal 3
-   [ ] 2022-11-28: Refine EDA and Prediction Results
-   [ ] 2022-12-5: [Final-Term
    Presentation](https://docs.google.com/presentation/d/1fAGY39dlRlgnB0LcdUKl_IA3Eaj7grqB/edit?usp=sharing&ouid=103328889489861986880&rtpof=true&sd=true)
-   [ ] 2022-12-16: [Final
    Delivery](https://docs.google.com/presentation/d/1fAGY39dlRlgnB0LcdUKl_IA3Eaj7grqB/edit?usp=sharing&ouid=103328889489861986880&rtpof=true&sd=true)

<p align="right">

(<a href="#readme-top">back to top</a>)

</p>

<!-- CONTACT -->

## Contact

-   Erqian Xu:
    [exu6\@u.rochester.edu](mailto:exu6@u.rochester.edu){.email}

-   Beilei Guo:
    [bguo5\@u.rochester.edu](mailto:bguo5@u.rochester.edu){.email}

-   Zhaoxuan Hu:
    [zhu21\@ur.rochester.edu](mailto:zhu21@ur.rochester.edu){.email}

-   Xinxuan Lu:
    [xlu39\@ur.rochester.edu](mailto:xlu39@ur.rochester.edu){.email}

-   Ziyue Yang:
    [zyang43\@ur.rochester.edu](mailto:zyang43@ur.rochester.edu){.email}

<p align="right">

(<a href="#readme-top">back to top</a>)

</p>

<!-- ACKNOWLEDGMENTS -->

## Acknowledgments

-   Lisa Altman and other GIDS advisors
-   Professor Ajay Anand
-   Professor Cantay Caliskan
-   TAs (Theodore Chapman & Nefle Nesli Oruc)

<p align="right">

(<a href="#readme-top">back to top</a>)

</p>

<!-- MARKDOWN LINKS & IMAGES -->

<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
