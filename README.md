# project
<img width="202" alt="0" src="https://github.com/user-attachments/assets/52e56065-16b7-48d7-b52b-92c3a4191beb">

After you start Docker Desktop for the first time, make sure to click on preferences and select appropriate memory for Docker to run, otherwise it might throw issues with a ML/DL library you install in the future that ends up needing more memory. 

To create the requirements file, run the following:

>> pipenv run pip freeze > requirements.txt

The project structure in the repo is important before you construct the dockerfile. If it looks like this:
<img width="140" alt="11" src="https://github.com/user-attachments/assets/0da0f269-a204-41c5-9c80-c289d1cec837">

Ensure you make your dockerfile while outside the app directory. A basic dockerfile looks like this:
<img width="232" alt="22" src="https://github.com/user-attachments/assets/42f8a3f7-7dfd-40d9-ac37-edca36ff80fb">

<img width="260" alt="33" src="https://github.com/user-attachments/assets/c84be373-052a-400c-bbd3-9f07141b987e">

If the humnan-readable docker image is tagged or named as 'rps', we build the docker image by running:
<img width="125" alt="44" src="https://github.com/user-attachments/assets/835ae4a8-3e7b-426a-859c-deee9595fd2f">
with a dot at the end of the command. 
The . at the end of docker build command indicates that Docker should look for the Dockerfile in our current directory.
[The tag might as well have a version and versioned name.]


Navigate to browser localhost:8501 to see the web app in action. 
For more, read <https://docs.docker.com/guides/docker-overview/>


