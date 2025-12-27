# Postman API Automation Integration with Github Actions #

This Repository is a demonstration for POC for integrating postman tests with github actions. The Tests are written in postman and they are executed onm the VM with the help of newman-reporter-htmlextra.
Github Actions will trigger the project execition on every push to the main branch. you can also execute the project manually using workflow_dispatch. The Projects runs on a scheduled time with the help of the cron job.

The HTML reports is archieved and kept in the artifact section for the team to download it. Along with that can view the report directlyt from the github page : https://laxmikantjava.github.io/Phoenix-Inwarranty-flow/
The Latest report is mailed to the team members using GMAIL SMPT


## About Me ##
Hi My Name is Jatin Sharma. I have 6.10 years of experience in Automation Testing. My Skillset includes UI Automation with Selenium Webdriver, Playwright and for API testing I used Rest Assured and Postman.
You can connect with me over: https://www.linkedin.com/in/laxmikant-y-223723122/

## Testing Coverage ##
1. Happy Flow Testing
2. Negative Testing and Edge Case Testing
3. Token Testing
4. Data driven Testing with CSV
5. Schema Validation
6. Secrets Managment with Github Secrets

## Tech Stack ##
1. Postman
2. Nodejs 22v
3. Newman
4. Newman-Reporter-Htmlextra
5. Github Actions
6. Gmail SMtp
7. Github Pages
8. CSV for Data Driven Testing
9. AWS-EC2 instance for Self hosted github runner.

## Github Pages ##
You can directly view the latest test report of the postman Test at the Github page : https://laxmikantjava.github.io/Phoenix-Inwarranty-flow/

### HTML Report #
   The Report will be created in the newman folder
   
   ![Postman Report](https://github.com/Laxmikantjava/Phoenix-Inwarranty-flow/blob/Static-content/Newman-Report.png)

## Postman Structure ##
```
Phoenix-Inwarranty-flow
├─ Inwarranty-flow-Collection.postman_collection.json # Collection File
├─ QA.postman_environment.json # environment File
└─ testdata.csv  # Testdata File

```

## How to run the Project? ##
You can run the project on your local system for that.
1. Clone the Project on the Local System: https://github.com/Laxmikantjava/Phoenix-Inwarranty-flow.git
2. Install Nodejs and NPM from https://nodejs.org/en
3. Install Newman using ```npm install -g newman```
4. Install Newman-reporter-htmlextra ``` npm install -g newman-reporter-htmlextra```
5. Run the Newmna cmmand:
    
           ```newman run 'Inwarranty-flow-Collection.postman_collection.json' \
          -e QA.postman_environment.json \
          -r cli,htmlextra \
          --reporter-htmlextra-export ./newman/index.html```
  

   
