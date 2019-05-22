# Predicting Usefulness of Code Review Comments using Textual Features and Developer Experience

Accepted Papers at MSR 2017
-------------------------------------------
```
Predicting Usefulness of Code Review Comments using Textual Features and Developer Experience
Mohammad Masudur Rahman, Chanchal K. Roy, and Raula G. Kula
```
**Download this paper:**  [<img src="http://homepage.usask.ca/~masud.rahman/img/pdf.png"
     alt="PDF" heigh="16px" width="16px" />](http://homepage.usask.ca/~masud.rahman/papers/masud-MSR2017a.pdf)

```
Impact of Continuous Integration on Code Reviews
Mohammad Masudur Rahman and Chanchal K. Roy
```
**Download this paper:**  [<img src="http://homepage.usask.ca/~masud.rahman/img/pdf.png"
     alt="PDF" heigh="16px" width="16px" />](http://homepage.usask.ca/~masud.rahman/papers/masud-MSR2017b.pdf)


**Abstract:**  Although peer code review is widely adopted in both commercial and open source development, existing studies suggest that such code reviews often contain a significant amount of non-useful review comments. Unfortunately, to date, no tools or techniques exist that can provide automatic support in improving those non-useful comments. In this paper, we first report a comparative study between useful and nonuseful review comments where we contrast between them using their textual characteristics and reviewers’ experience. Then, based on the findings from the study, we develop RevHelper, a prediction model that can help the developers improve their code review comments through automatic prediction of their usefulness during review submission. Comparative study using 1,116 review comments suggested that useful comments share more vocabularies with the changed code, contain salient items like relevant code elements, and their reviewers are generally more experienced. Experiments using 1,482 review comments report that our model can predict comment usefulness with 66% prediction accuracy which is promising. Comparison with three variants of a baseline model using a case study validates our empirical findings and demonstrates the potential of our model.

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
**Prediction Model**
-   [Feature Set](https://drive.google.com/open?id=0B9GerXe2gpyFYldQZW1YcW13SUk)
-   [Evaluation dataset](https://drive.google.com/open?id=0B9GerXe2gpyFZ1g1b1dfQ0szT00)
-   [Validation dataset](https://drive.google.com/open?id=0B9GerXe2gpyFWVpYSVRYazRZNmc)
-   [RevHelper Model (Training & Testing)](https://drive.google.com/open?id=0B9GerXe2gpyFejdUeE1zUG80RTg)
-   [RevHelper Model (Validation)](https://drive.google.com/open?id=0B9GerXe2gpyFeURVN04wZ1h2dGc)

**Auxiliary Items for Replication:**
-   Stop words
-   Python keywords
-   Readability Ease calculator library
-   Regex for question identification:  `"[?]($|\s)"`  and sentence identification:  `"[?!.]($|\s)"`
-   Regex for code element identification:  ``"`{3}[\S+\s+]+`{3}|`[\S+]+`|`[\S+\s+]+`"``
-   [GitHub API librarry](http://github-api.kohsuke.org/)
-   [Git Bash](https://git-scm.com/)


**Model Training & Testing**
-   All useful comments (618)
-   All non-useful comments (498)
  
**Model Validation & Case study**
-   CS (81)
-   SM (99)
-   MS (99)
-   SR (87)
-   All useful comments (262)
-   All non-useful comments (104)

## Please cite our work as
```
@inproceedings{msr2017masud, 
author = {Rahman, M. M. and Roy, C. K. and Kula, R. G. }, 
title = {{Predicting Usefulness of Code Review Comments using Textual Features and Developer Experience}}, 
booktitle = {Proc. MSR}, 
year = {2017}, 
pages = {215--226} }
```
**Download this paper:**  [<img src="http://homepage.usask.ca/~masud.rahman/img/pdf.png"
     alt="PDF" heigh="16px" width="16px" />](http://homepage.usask.ca/~masud.rahman/papers/masud-MSR2017a.pdf)


Do you also want to check [CORRECT](https://github.com/masud-technope/CORRECT-Replication-Package-ICSE2016)?
--------------

## Something not working as expected?

Contact:  **Masud Rahman**  ([masud.rahman@usask.ca](mailto:masud.rahman@usask.ca))

OR

Create an issue from  [here](https://github.com/masud-technope/RevHelper-Replication-Package-MSR2017/issues/new)

