<!-- PROJECT LOGO -->
<div align="center">
  <a href="https://github.com/github_username/repo_name">
    <img src="images/gids.jpeg" alt="Logo" width="280" height="80">
  </a>

<h3 align="center">GIDS:Understanding Masters' Applicant Pool</h3>

  
</div>



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

<div align="center">
  <a href="https://github.com/github_username/repo_name">
    <img src="images/gids2.jpg"  width="280" height="200">
  </a>
 
</div>
Sponsor: [GIDS](https://www.sas.rochester.edu/dsc/)

Project Link: [GIDS github](https://github.com/Egret-Lu/GIDS)

This report presents our analysis of selection criteria and application procedure for graduate school admission across three programs from the Arts, Sciences, and Engineering (AS&E) program at the University of Rochester, including Computer Science, Data Science, and Electronic Chemical Engineering. Specifically, it unfolds applicants' characters in three ways: applicants' demographic information, applicants' behavior, and applicants' decision. It begins with an overview of the dataset, followed by exploratory data analysis results, and concludes with predictive models. Techniques to handle missing values that are not completely at random and algorithms to overcome data imbalance are explored. Implications and limitations are also discussed in this report. 

Codes of the project is mainly based on python programming. 

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With
* pandas
* numpy
* matplotlib
* seaborn
* nltk
* sklearn
<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

<!-- Install modules -->
### Installation

Install required modules in terminal ```pip install -r requirements.txt```


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

1. Data File: unzip DATA.zip
2. User Profile Analysis: EDA_applicant_profile.ipynb
3. User Behavior Analysis: EDA_applicant_behaviour.ipynb
4. Prediction Model: Classification_models.ipynb

For more explanations, please refer to the [Report](https://www.overleaf.com/read/bqbxfrycbmhf)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- Figure -->
## Figure List

Figures shows in the [report](https://www.overleaf.com/read/bqbxfrycbmhf)

1. EDA_applicant_profile.ipynb： Fig 1, 2, 3, 4, 5, 6, 7, 25, 27
2. EDA_applicant_behaviour.ipynb： Fig 8, 9, 10, 11, 12, 13, 14, 26
3. Classification_models.ipynb： Fig 19,20,21, 22, 23, 24

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- outline -->
## Code Outline

Here is the outline of our codes

### EDA

1. EDA_applicant_profile.ipynb： 
  - Outline:
    - Who applies to each of our programs? 
    - What is the makeup of those who get admitted and those who accept our offer.
    - Using application data, analyze master forn different programs
    - Compare the data of admitted, rejected, accepted or denied students.
    - Common info age, M/F, URM, international, GPA, TOEFL/IETLS, GRE
    - Trends of the applicants
  - Main Figures:
      - Gender of Admitted Students Grouped by Three Programs
      - Percentage of Female across Years
      - Top Birth States of Our Applicants
      - Average GPA score of Our Applicans
      - Age Distribution of Admitted Applicants
      - Career Plan for All Applicants
    
2. EDA_applicant_behaviour.ipynb： 
  - Outline
    - Derive insights on the application timeline
    - Understand the types of institutions/programs people are choosing to attend.
  - Main Figures:
      - The Number of Completed References before Submission
      - Timeline of Submitting Applications
      - Trend of Admitted Data Science Students' Interest
      - rend of Admitted DS Students Heard About UR 
      - Where do Applicants who doesn't Attend UR Go
    
### Model 

Classification_models.ipynb： 

1. Data Preprocessing:
  - Missing Data Handling: 
      -Deletion: Missing >10% 
      - Imputation: Missing not completely fill -1
  - Feature Engineer:
    - Focus on features that unsubmitted ones did not fill in 
    - Generate new variables based on existed ones (e.g. number of previous jobs, completed references, previous institutions and other applied colleges)                     
  - Data Transformation:
    - Categorical variables: Transform to one-hot encoder (dummy variables)
    - Normalization: MinMaxScaler      

2. Predict which students will submit/un submit our offer of admissions?
    - Gaussian Mixture
    - SMOTE+ Linear Regression
3. Predict which students will accept/decline our offer of admissions?
    - SVM (polynomial of degree 2) 
    - SVM (RBF kernel)
    - Gaussian Naive Bayes
    - Gaussian Process
    - K Nearest Neighbour
    - Quadratic Discriminant Analysis


<!-- ROADMAP -->
## Roadmap

- [ ] 2022-9-28: Project Charter
- [ ] 2022-10-17: Goal 1 & Goal 3 Merging Datasets
- [ ] 2022-10-26: Goal 2 EDA
- [ ] 2022-11-2:[Mid-Term Presentation](https://docs.google.com/presentation/d/1Yqd0spkCZES3Iia8LSHgBdiUbmiSxVwrGWw0FAfmaII/edit?usp=sharing)
- [ ] 2022-11-16: EDA Goal 2 Prediction & Goal 3
- [ ] 2022-11-28: Refine EDA and Prediction Results
- [ ] 2022-12-5: [Final-Term Presentation](https://docs.google.com/presentation/d/1fAGY39dlRlgnB0LcdUKl_IA3Eaj7grqB/edit?usp=sharing&ouid=103328889489861986880&rtpof=true&sd=true)
- [ ] 2022-12-16: [Final Delivery](https://docs.google.com/presentation/d/1fAGY39dlRlgnB0LcdUKl_IA3Eaj7grqB/edit?usp=sharing&ouid=103328889489861986880&rtpof=true&sd=true)




<p align="right">(<a href="#readme-top">back to top</a>)</p>




<!-- CONTACT -->
## Contact
If you have any questions, please contact our group members:

- Erqian Xu: exu6@u.rochester.edu

- Beilei Guo: bguo5@u.rochester.edu

- Zhaoxuan Hu: zhu21@ur.rochester.edu

- Xinxuan Lu: xlu39@ur.rochester.edu

- Ziyue Yang: zyang43@ur.rochester.edu


<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* Lisa Altman and other GIDS advisors
* Professor Ajay Anand
* Professor Cantay Caliskan
* TAs (Theodore Chapman & Nefle Nesli Oruc)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/github_username/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/github_username/repo_name/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/github_username/repo_name.svg?style=for-the-badge
[forks-url]: https://github.com/github_username/repo_name/network/members
[stars-shield]: https://img.shields.io/github/stars/github_username/repo_name.svg?style=for-the-badge
[stars-url]: https://github.com/github_username/repo_name/stargazers
[issues-shield]: https://img.shields.io/github/issues/github_username/repo_name.svg?style=for-the-badge
[issues-url]: https://github.com/github_username/repo_name/issues
[license-shield]: https://img.shields.io/github/license/github_username/repo_name.svg?style=for-the-badge
[license-url]: https://github.com/github_username/repo_name/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
