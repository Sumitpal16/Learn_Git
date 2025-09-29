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
-- Create an SSH key for GitHub Actions → EC2
2. ⁠issue ssh commands to pull the code on ec2 instance
-- Add GitHub Secrets (repo → Settings → Secrets and variables → Actions)
3. ⁠issue ssh command to run your bash script
-- Add the workflow to your repo -- Create .github/workflows/deploy-ec2-static.yml
-- Push & test

You can make bash script part of your GitHub repo for simplicity so that the application code (html files) and deployment code (bash script) are maintained in a single repo.

NOTE :: Before making any CI/CD pipeline always ensure u are able to manually run all your flow elements. One of the core parts of this pipeline is to run command by ssh, not by logging into the terminal but to issue command without entering the terminal.

--------- DAY 3 --------- 

1. Run locally and make requests via postman
2. ⁠deploy manually on ec2 what are the various ways there are at least 3 ways it's just a hint each has pro and cons
3. ⁠deploy with script
4. ⁠deploy with GitHub action.
