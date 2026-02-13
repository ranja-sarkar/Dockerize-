

To create the requirements file, run the following:

>> pipenv run pip freeze > requirements.txt

Ensure you make your dockerfile while outside the app directory. A basic dockerfile looks like this:
<img width="232" alt="22" src="https://github.com/user-attachments/assets/42f8a3f7-7dfd-40d9-ac37-edca36ff80fb">

<img width="260" alt="33" src="https://github.com/user-attachments/assets/c84be373-052a-400c-bbd3-9f07141b987e">

If the human-readable docker image is tagged or named as 'rps', we build the docker image by running:
<img width="125" alt="44" src="https://github.com/user-attachments/assets/835ae4a8-3e7b-426a-859c-deee9595fd2f">
with a dot at the end of the command. 
The . at the end of docker build command indicates that Docker should look for the Dockerfile in our current directory.
[The tag might as well have a version and versioned name.]


Navigate to browser localhost:8501 to see the web app in action. 
For more, read <https://docs.docker.com/guides/docker-overview/>

If you want to use GitHub Actions and Azure App Services for your production then follow this:

<img width="610" alt="github_actions" src="https://github.com/user-attachments/assets/12947465-789f-4061-9d4b-6eb57d3b1250">

For CI/CD this is preferred. 

<img width="595" alt="CI_CD" src="https://github.com/user-attachments/assets/c6f9dcbc-67b3-4a6b-b093-1aadd8ff357e">

There're different testing types which are performed in different environments. Smoke testing and regression testing are done in the deployed environments.   
Data migration testing is done in staging environment, system integration testing (SIT) in SIT environment, performance testing is done in SIT and UAT environments, 
funtional testing in QA environment. 

<img width="226" alt="Tests" src="https://github.com/user-attachments/assets/524f1eb4-3576-4235-bcd6-85c908593d37">
