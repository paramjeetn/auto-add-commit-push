# auto-add-commit-push
Using Linux bash scripting to automatise the process of // git add .  // git commit -m " " // git push origin branch

Step 1:- Go to repo folder on local machine  \
Step 2:- From your repo go to terminal by right click and open in terminal . \
step 3:- type      sudo gedit repo_name_autopush.sh        , then and give the password \
Step 4: Vim editor opens up automatically \
paste the code with nessecary changes 


git add .

echo 'Enter the commit message:' \
read commitMessage

git commit -m "$commitMessage" 

echo 'Enter the name of the branch:' \
read branch

git push origin $branch

exit 

read



## necessary changes to do :- 
if you have a single branch then you can just delete 5th and 6th lines and in 7th line delete $branch and write your branch name there wihtout $ /// just write branch name only. 

Step 5:- press ctrl+s , and exit the file ( ctrl+w two times will do)  \
Step 6:- from the repo open terminal  \
Step 7:- type  sudo chmod +x repo_name_autopush.sh            
step 8:- give password , DONE \
Final step : - just right click on the sh file and then click run as program , it will ask for commit message then press enter , also do same if ask branch name give the branch name and enter. 


# NOW YOU CAN COMMIT AND PUSH WITH ONE CLICK
