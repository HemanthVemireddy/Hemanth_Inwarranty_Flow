
# Postman API Automation Integration with Github Actions. #

This repository is a demonstration for POC for integrating postman tests with github actions. The Tests are written in Postman and they are executed on the VM with the help of newman and newman-reporter-htmlextra.

Github Actions will trigger the project execution on every push to the main branch. You can also execute the project manually using workflow_dispatch. The Projects runs on a scheduled time with the help of the cron job.

## About Me ##
Hi My name is Hemanth. I have 5 Years of experience in Automation Testing. My skill set include UI Automation with Selenium Webdriver and API Testing I use Postman and Rest Assured with Java, Mobile Automation Appium with java.
you can connect with me over : www.linkedin.com/in/hemanth-vemireddy

## Testing Coverage ##
1. Happy Flow Testing
2. Negative Testing and Edge Case Testing
3. Token Testing
4. Data Driven Testing with CSV
5. Schema Validation
6. Secrets Management with Github Secrets

## Project Structure ##

```
Hemanth_Inwarranty_Flow
├─ Hemanth_Inwarranty-flow_Collection.postman_collection.json # Collection file
├─ QA.postman_environment.json # Environment file
└─ testData.csv # Data file

```

## Tech Stack ##

1. Tech Stack 
2. Postman
3. Nodejs 22v
4. Newman
5. Newman-Reporter-Htmlextra
6. Github Actions
7. Gmail SMTP
8. Github Pages
9. CSV for Data Driven Testing
10. AWS-EC2 instance for Self hosted github runner.

# Github Pages #

You can directly view the latest test report of the Postman Test at the Github Page Link:
https://github.com/HemanthVemireddy/Hemanth_Inwarranty_Flow

## How to run the Project? ##

1. You can run the project on your local system for that:
2. Clone the Project on Local System: https://github.com/jatin99/Phoenix-Inwarranty-Flow.git
3. Install Nodejs and NPM from https://nodejs.org/en
4. Install Newman using npm install -g newman
5. Install Newman-reporter-htmlextra using npm install -g newman-reporter-htmlextra
6. Run the Newman Command:
    ```
    newman run 'Inwarranty-flow Collection.postman_collection.json' \
    -e QA.postman_environment.json \
    -d testdata.csv \
    -r cli,htmlextra \
    --reporter-htmlextra-export ./newman/index.html
    ```

## HTML Report ##
The Report will be created in the newman folder.
