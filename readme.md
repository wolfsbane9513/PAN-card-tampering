Step to run application:

Step 1:	Create the copy of the project.<
Step 2: Open command prompt and change your current path  to folder where you can find 'app.py' file.
Step 3: Create environment by command given below- conda create -name <environment name>
Step 4: Activate environment by command as follows- conda activate <environment name>
Step 5: Use command below to install required dependencies-python -m pip install -r requirements.txt
Step 6: Run application by command;python app.py
You will get url copy it and paste in browser.
Step 7: You have sample_data folder where you can get images to test.
  
When deploying on heroku-
Ensure
1.Add an Aptfile in your project directory and add the below file
libsm6
libxrender1
libfontconfig1
libice6
NOTE: Aptfile should not have any .txt or any other extension. Just like the Procfile

2.Push the edited code to Github

3.In heroku dashboard,
goto your-app 
--> settings 
--> buildpacks 
--> add buildpacks 
--> https://github.com/heroku/heroku-buildpack-apt.git

copy and paste this link 
--> add buildpack

4.Deploy your app
