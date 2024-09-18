# COMP-390-GIT-Setup-Instructions

## Install git command line tool
### MacOS 
Open terminal and type the following command 
```
brew install git
```
### On Windows 
1. Go to the official Git website. 
2. Click on Download for Windows to download the latest version of Git. 
3. Once the file is downloaded, open it to run the Git installer. 
4. In the setup window, read the license agreement and click Next to accept it. 
5. Choose the destination folder where you want to install Git. The default location is usually fine. Click Next. 
6. Leave the default options selected, including: 
  - Additional icons (optional) 
  - Git Bash Here and Git GUI Here (important for right-click options)
  - Git LFS (Large File Support) (optional). Click Next. 
7. Choose the default start menu folder or change it if needed. Click Next. 
8. Click Next 
9. Click Finish

## Verify Installation
Run command in terminal on MacOS or Git Bash on Windows
```
git --version
```

## Create a new repository
1. Login to github.com
2. Click on `+` on the upper right corner and select "New Repository"
![](https://github.com/ShantalaGaitonde/comp390-git-instructions/blob/main/create-button-location.png?raw=true)
3. Name the repository hello-world.
4. Add a description if you like.
5. Ensure the `Public` is selected.
6. Check the box that says Add a README file.
![](https://github.com/ShantalaGaitonde/comp390-git-instructions/blob/main/create-repository.png?raw=true)
7. Click on "Create Repository".

## Checkout repository to your local machine
Run the following command using Terminal on macOS and Git Bash on Windows
```
git clone https://github.com/your-username/hello-world.git 
cd hello-world
```
### Verify project
```
git status
```

## Create a new branch
Branches allow you to work on a feature or fix without affecting the main project. 

1. Create a branch 
```
git checkout –b feature-branch 
```
2. Push the branch to remote repository
```
git push --set-upstream origin feature-branch
```

## Make Changes and Push to the Branch
Open PyCharm and open the cloned hello-world project. 

1. Create a python file called main.py and add the following line to the file 
```
print(“Hello World!”) 
```
2. Go to Terminal on MacOS or Git Bash on Windows, navigate to the root directory of your project and run the following commands to push your changes to GitHub. 
```
git add . 
git commit -m "Added main.py" 
git push
```

## Create a Pull Request
1. Go to your repository on GitHub. 
2. You will see a Compare & pull request button appear after pushing your branch.
![](https://github.com/ShantalaGaitonde/comp390-git-instructions/blob/main/create-pull-request.png?raw=true)
3. Click on it. 
4. Review the changes, add a title, and a description for the pull request. 
5. Click Create pull request.

## Merge to `main`
1. Once your pull request has been reviewed and approved (even if it's just you), click the Merge pull request button. 
2. After merging, you can delete the feature branch by clicking Delete branch. 
