# Predicting Usefulness of Code Review Comments using Textual Features and Developer Experience

Accepted Papers at MSR 2017
-------------------------------------------
```
Predicting Usefulness of Code Review Comments using Textual Features and Developer Experience
Mohammad Masudur Rahman, Chanchal K. Roy, and Raula G. Kula
```
**Download this paper:**  [<img src="http://web.cs.dal.ca/~masud/img/pdf.png"
     alt="PDF" heigh="16px" width="16px" />](http://web.cs.dal.ca/~masud/papers/masud-MSR2017a.pdf)

```
Impact of Continuous Integration on Code Reviews
Mohammad Masudur Rahman and Chanchal K. Roy
```
**Download this paper:**  [<img src="http://web.cs.dal.ca/~masud/img/pdf.png"
     alt="PDF" heigh="16px" width="16px" />](http://web.cs.dal.ca/~masud/papers/masud-MSR2017b.pdf)


**Abstract:**  Although peer code review is widely adopted in both commercial and open source development, existing studies suggest that such code reviews often contain a significant amount of non-useful review comments. Unfortunately, to date, no tools or techniques exist that can provide automatic support in improving those non-useful comments. In this paper, we first report a comparative study between useful and nonuseful review comments, where we contrast them using their textual characteristics and reviewers’ experience. Then, based on the findings from the study, we develop RevHelper, a prediction model that can help developers improve their code review comments through automatic prediction of their usefulness during review submission. A comparative study using 1,116 review comments suggested that useful comments share more vocabulary with the changed code, contain salient items like relevant code elements, and that their reviewers are generally more experienced. Experiments using 1,482 review comments report that our model can predict comment usefulness with 66% prediction accuracy, which is promising. Comparison with three variants of a baseline model using a case study validates our empirical findings and demonstrates the potential of our model.

Comparative Study
-----------------------------------
The review comments below are used for our comparative study between useful and non-useful comments:
-   **CS** (256)
-   **SM** (281)
-   **MS** (288)
-   **SR** (291)
-   All useful comments (618)
-   All non-useful comments (498)

Review Usefulness Prediction
-----------------------------------  
**Prediction Models**
- ```Model-python```
     -  revhelper-model_rf.ipynb
     -  revhelper-model-rf-validator.ipynb
- ```Model-R (old)```
     -  revhelper-model_rf.r
     -  revhelper-model-rf-validator.ipynb

**Auxiliary Items for Replication:**
-   Stop words
-   Python keywords
-   Readability Ease calculator library: ```readability.jar```
-   Regex for question identification:  `"[?]($|\s)"`  and sentence identification:  `"[?!.]($|\s)"`
-   Regex for code element identification:  ``"`{3}[\S+\s+]+`{3}|`[\S+]+`|`[\S+\s+]+`"``
-   [GitHub API library](https://github.com/hub4j/github-api)
-   [Git Bash](https://git-scm.com/)

**Model Training & Testing**
-   All useful comments (618)
-   All non-useful comments (498)
-   modeldata-training-and-testing.csv
  
**Model Validation & Case study**
-   CS (81)
-   SM (99)
-   MS (99)
-   SR (87)
-   All useful comments (262)
-   All non-useful comments (104)
-   model-validation-data.csv

## Please cite our work as
```
@inproceedings{msr2017masud, 
author = {Rahman, M. M. and Roy, C. K. and Kula, R. G. }, 
title = {{Predicting Usefulness of Code Review Comments using Textual Features and Developer Experience}}, 
booktitle = {Proc. MSR}, 
year = {2017}, 
pages = {215--226} }
```
**Download this paper:**  [<img src="http://web.cs.dal.ca/~masud/img/pdf.png"
     alt="PDF" heigh="16px" width="16px" />](http://we.cs.dal.ca/~masud/papers/masud-MSR2017a.pdf)


Do you also want to check [CORRECT](https://github.com/masud-technope/CORRECT-Replication-Package-ICSE2016)?
--------------

## Something not working as expected?

Contact:  **Masud Rahman**  ([masud.rahman@usask.ca](mailto:masud.rahman@usask.ca))

OR

Create an issue from  [here](https://github.com/masud-technope/RevHelper-Replication-Package-MSR2017/issues/new)

