# dot-net-iot-project


ehhh whatever, if this repo gives me trouble I can always delete it and create a new one
dotnet on vscode tutorial: https://code.visualstudio.com/docs/languages/dotnet

even better tutorial: https://learn.microsoft.com/en-us/azure/app-service/quickstart-dotnetcore?tabs=net70&pivots=development-environment-vscode 

INCLUDE PLAYWRIGHT HERE TO DO WEB SCRAPING OF SOME WEBSITE AND THEN TURN IT INTO A RANDOM JSON MESSAGE TO BE SENT TO AZURE API MANAGEMENT, MAYBE I CAN EVEN USE OPENAI API FOR THIS??? WE'LL SEE. MAYBE AZURE FUNCTION WILL INCLUDE THE OPENAI API TO MAKE SENSE OF THE INFORMATION I SENT IT

I will be using this project to gain fimiliarity with C# and other dot net things as it relates to cloud    ALSO THE TITLE WILL BE CHANGED TO .NET BASED CLOUD-NATIVE FRONTEND
ooooh this could be the frontend of the alzhiemer's project that is written in c# instead, I could create a login and stuff, and the output will be a json that through azure functions as an api sends the json data to the distributed data pipeline (the docker containers in that pipeline will be in a kubernetes cluster pod and is deployed using terraform)

So terraform will be in my work experience resume and this will be in my projects section in resume

quick test

another quick test

## process on how I'll go about the project for this repository

1. create a c# azure web app and download the code and edit the code such that sends a json message (actually when I create the web app is can be created as a docker container so maybe write this as a container?? idk we'll see)  

** also if I do create this as a docker container then I can push it to azure container service and give permission access for azure function to run it or something like that **  

** so it also turns out there is github integration for the web app, in that case it doesn't need to be a docker container, i can do ci/cd tests on the code using github actions **
2. create azure api management to catch that message and parse it and sends it to an azure function that will then send it to me as an email notification (an azure function will be configured as an api in azure api management)
3. if errors come up then debug (use github actions for CI/CD tests to debug) 
4. Maybe create a simple frontend using streamlit to display the results of/using azure function that became an api
5. Monitor everything on azure monitor and maybe set up prometheus to create some cool dashboards


## process on how I'll go about the project for the combined project with kubernetes, ingress and terraform

1. create a c#/.net container that sends a message to an ingress controller (and push to azure container registry)
2. create azure api management to catch that message and parse it and sends it to an azure function that will then send it to me as an email notification (an azure function will be configured as an api in azure api management)
3. prototype a kubernetes pod and put the container in it and use ingress and try to send to azure api managemtn
4. if errors come up then debug
5. test everything in terraform I guess (this will be in the other repository though)

## notes

Yeah do something with c# and playwright in this, absolutely forget about golang tbh, it sucks and I have no idea where to use golang

!!! CREATE A DOCKER HEALTH CHECK USING C#, and use github actions to do CI/CD and c# and JUST USE THE POSTGRESQL DATABASE CONTAINER I USED BEFORE AS TESTING!!!
follow this tutorial:
https://www.youtube.com/watch?v=tj5ZCtvgXKY&ab_channel=MilanJovanovi%C4%87 


HONESTLY, THIS SHOULD JUST BE AN ADD ON FOR CLOUD PROJECT INSTEAD OF
ITS OWN THING

In that case producer will be .net written in c# and consumer will be written in golang

Or it can be the other way around, consumer will be .net written in c# and producer will be written in golang






follow this tutorial too if needed: https://medium.com/geekculture/integration-test-with-docker-and-net6-564cb4922cfd 

also do it with test containers dot net : https://github.com/testcontainers/testcontainers-dotnet 

Huh this could be a TEST CONTAINERS + .NET + GITHUB ACTIONS PROJECT

so the process is: .net integration test is written and will be deployed inside of testcontainer which will be created through github actions during a git push

esentially replicate this: https://www.youtube.com/watch?v=ZLwZ3Cdt9Vs (wriiten documentation here: https://testcontainers.com/guides/testing-an-aspnet-core-web-app/)


If time is available then do some thing with playwright
If i do use playwright, then I can create a simple playwright script that gets the website data in puts them in the postgresql database. Pretty good plan tbh. I'm gonna execute this going forward. Playwright can go on the data engineering extern on resume, and c# testing can go on the novo project on basic resume

I will be using playwright here, I'll do come automation stuff with it I guess, maybe even create a bot
Or I could do some kind of api testing with playwright, I'll see if that is the best course of action for this project

https://www.youtube.com/watch?v=3s-RfwvijpY 
^^copy this video

quick test
