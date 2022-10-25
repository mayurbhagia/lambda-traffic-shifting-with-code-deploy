This repo is to create a Hello World Python project and test Lambda traffic shifting from one version to another using AWS Code Deploy


Credit to https://github.com/adhorn/aws-lambda-sam-application/

Either you can clone this repo and perform the test

Alternatively if you dont want to clone this repo and want to learn by doing it yourself from sratch, follow below steps:

Step 1 - Install SAM CLI, Python3.7 and Git
Step 2 - sam init -o ./newdevdaydemo -n new-helloworld-app --runtime python3.7
Step 3 - Now update the template.yaml and folder of pre-traffic-hook and copy the files from this git to your local folder
Step 3 - sam build --use-container
Step 4 - same deploy --guided
Step 5 - sam local invoke HelloWorldFunction --event events/event.json or sam local start-api --debug
