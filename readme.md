# wpEngine Continuous Integration Template

## Initial wordpress setup
1.  Login to [wpengine](wpengine.com).  
2.  Navigate to the backup point of the production branch on wpengine
3.  create a backup and download full version of it
4.  Unzip the backup and 
## Gulp setup

## [CircleCI](https://circleci.com/) setup

All circleci settings will be housed in _./.circleci/config.yml_
1.  For each of the wpengine site branches (production, staging and development), navigate to the Git push page and enter ssh information.  For more info on setting up a ssh key, see [here](https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
2. Copy ssh key to clipboard
3. within wpengine, navigate to the *Git push*; Enter Developer name, paste ssh key to the SSH public,  and click *Add Developer*.  This will generate a fingerprint.
4.  copy fingerprint and add to circleci/config.yml to the corresponding location.  
5.  Repeat these steps for each site (Production, Staging, Development)