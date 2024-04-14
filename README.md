# CERITA

## Step 1 - Clone the template repository


git clone git@github.com:nsengnk/cerita.git
cd cerita

## Dev process

```mermaid
graph TD
    new_need[new demand or evol]
    git_new_issue[1. git - create a new issue]
    git_new_branch[2. git - create new branch]
    develop[3. Develop and commit your devs into your branch]
    doc[4. update the documentation if needed]
    check[5. Check final CICD]
    push[6. Push your branch and create a merge request (the reviewer is the project manager)]
    new_need --> git_new_issue
    git_new_issue --> git_new_branch
    git_new_branch --> develop
    develop --> doc
    doc --> check
    check --> push
```
