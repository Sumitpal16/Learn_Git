--------- DAY 1 --------- 

1. locally update the index.html with any thing
-- Updated index.html in locally (VS Code) 

2. Push the changes to git.
-- git push origin master

3. pull the changes in the EC2 instance.
-- connect EC2 and git pull (code)

4. Write a bash script to copy the new files to the /var/www/html
-- Bash script in EC2 with source Git1 (project) and dest  /var/www/html
-- Run script

5. see if those changed or not
-- Refresh browser

--------- DAY 2 --------- 

Create a CI/CD pipeline using GitHub actions

Flow:
1. Run the action on push to your branch
2. ⁠issue ssh commands to pull the code on ec2 instance
3. ⁠issue ssh command to run your bash script

You can make bash script part of your GitHub repo for simplicity so that the application code (html files) and deployment code (bash script) are maintained in a single repo.
