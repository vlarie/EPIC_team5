## Workflow Procedures for Team EPIC

#### NOTE:  Until unique environment is developed for this project, work in PythonData virtual environment

To ensure receipt of notifications on repo
	
- Navigate to GitHub repo page `vlarie/EPIC_team5`
- Under the main header bar on the right, select the drop down next to the eyeball and change notifications to `Watching`
  - You may also want to `Star` the repo 


### Branch naming conventions
lowercase first initial of person working branch + CamelCase of task being worked on
- e.g. tRandLatLng (for Troy's branch creating random latitudes and longitudes), tPlotGeocodes (for Troy's branch plotting coordinates)

	
	
	
## Procedure for merging to master
#### NOTE:  Merging to master should occur when one of these conditions has been met:
1. The code being merged is vital to the function or completion of other parts of the project in development
2. The code being merged is fully functional, no longer in development, and will not need any more major changes

Please ensure one or more of these conditions is met before submitting a pull request.
	
	
	
### Create branch using established naming conventions
terminal method:
- Create new branch

`git branch <branch_name>`
- Command to move between branches

`git checkout <branch_name or master>`
- Create and switch to branch in one line

`git checkout -b <branch_name>`



### Complete work on branch 
Work on branch locally making commits often as code develops



### Push branch to GitHub
terminal method:
- Updates branch specified on GitHub

`git push origin <branch_name>`



### Pull request to merge to master
After branch work is complete and you want to merge to master, navigate to GitHub.com repository online
- From the `<>Code` tab click `New pull request`   OR   from the `Pull request` tab click `New pull request`
- Compare changes - `base: master`   <-   `compare: <branch_name>`
- Add Valerie (aka vlarie) as reviewer and anyone else applicable, like people working on similar code
- Assign yourself
- Write any comments or notes
- Click `Create pull request`



### Merge to master
- Valerie will receive a notification of pull request and review within 12 hours* 
  - (*if there are extenuating circumstances preventing this, Valerie will communicate to individual submitting for review)
- If there are any changes to be made, Valerie will submit those back to the individual to be addressed within 12 hours if possible
- If no changes need to be made, Valerie will merge branch to master
	
	
	
### Pull changes from master	
- When branches are merged to master, team members should receive notification via email
- Each person should then update their local repo to incorporate changes

terminal method:	
- First navigate to relevant repo folder 
  - If you have NOT made ANY changes locally whatsoever, use the following command

`git pull origin master`
  - If you have made commits on your local copy, using rebase will roll back your changes temporarily 
to first update your local copy to match current remote, then replay your changes onto the end

`git rebase origin/master`
#### NOTE: You may have to review differences/merge conflicts with this method


