# GitHub Actions Workflow Analysis

## 1. What triggers the workflow to run?

The workflow runs when code is pushed to the main branch, or when a pull request is made to the main branch.

## 2. What are the four main steps this workflow performs?

1. Chechout code Gets the project code
2. Validate HTML - Checks the html for errors
3. Checks links - Checks the HTML for links that dont work
4. Upload artifact - Prepares the website for getting deployed

## 3. What does the checkout code step do and why is it necessary? 

it gets the code from the repository so GitHub use the files. It is necessary because the other steps need access to all of the files

## 4. What is the purpose of environment configuration?

It sets tup the github pages environment for the deploymnet and provides the website's URL

## 5. How does this automated deployment improve reliability compared to manual deployment?

It performs the same checks everytime, which reduces human error and makes the process as a whole more consistent

## 6. What would happen if you pushed cde to a different branch?

If you push code to another branch, the workflow will not run. If you make a pull request to main, the test will run but the website will only be deployed after it is merged into main. 