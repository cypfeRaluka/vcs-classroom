How to contribute (recommended workflow)

Step 1: Clone the repo  
git clone https://github.com/philipobiorah/vcs-classroom.git  
cd vcs-classroom  

Step 2: Create a new branch  
Use your name in the branch:  
git checkout -b profile/firstname-lastname  

Example:  
git checkout -b profile/jane-doe  

Step 3: Create your profile file  
mkdir -p students  

Create and edit your file (choose ONE method):  

Mac/Linux:  
touch students/firstname-lastname.md  

Windows PowerShell:  
New-Item students\firstname-lastname.md -ItemType File  

Then open it in your editor (VS Code is fine) and paste the template.  

Step 4: Add and commit  
git add students/firstname-lastname.md  
git commit -m "Add student profile: Firstname Lastname"  

Step 5: Push your branch to GitHub  
git push -u origin profile/firstname-lastname  

Step 6: Open a Pull Request (PR) on GitHub  
Go to the repo on GitHub.  
Click Compare & pull request.  
Title: Add student profile: Firstname Lastname  
Click Create pull request.  

Peer review (Everyone)  
Before your PR is merged, you must review one other PR:  
Read their students/*.md file  
Leave 1 helpful comment (example: “Looks good, maybe add your GitHub username too.”)  

Helpful commands  
Check what changed:  
git status  

See your commit history:  
git log --oneline  

See all branches:  
git branch  

Pull latest updates:  
git pull  

Common mistakes and fixes  

I forgot to create a branch  
Create one and move your work onto it:  
git checkout -b fix/move-to-branch  

My branch is behind main  
Update your local main, then merge main into your branch:  
git checkout main  
git pull  
git checkout your-branch-name  
git merge main  
