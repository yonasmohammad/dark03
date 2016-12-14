### Getting started
>  **Todo:** Add q quick getting started guide that covers:
>
	>Introduction to:
	>	>1. Node Package Manager  [npm, ](https://www.npmjs.com "'node homepage") 
	>	>2. Gulp (Build Process) [gulp](http://gulpjs.com "intall scss")[npm bootraps](https://forums.meteor.com/t/the-way-to-use-bootstrap-4-from-npm-including-js-and-tether/23159 "download bootraps")
	>	>3. Nunjucks (Templating Language) [Nunjucks](https://mozilla.github.io/nunjucks/) 
	> >4. Bootraps (4.0) 	 [getting-started](http://getbootstrap.com/getting-started/) 
	> >5. Git  [git-main](https://git-scm.com/) 
	> >6. SASS (SCSS)  [Sass Basics](http://sass-lang.com/guide) 
### Installation
> #####**Node Package Manager**
 ``` npm install  ``` or   ```npm install --production ```
#####This will install node modules needed by app(adding  ``` --production  ``` param is optional if you will not use nodes as the server) Post install will execute these commands automatically:  ``` bower install  ``` and  ``` gulp uikit:install  ```

> #####**Gulp**
 ``` npm install --save gulp-install  ``` or   ```npm install --save-dev gulp-install ```
 >
		> **basic ussage**
		>	>```gulp watch:sass```
> Watch changes on the SCSS files and compiles it

#####It will run the command in the directory it finds the file, so if you have configs nested in a lower directory than your slushfile.js/gulpfile.js, this will still work.





### Npm - bootrap
```npm install --save bootstrap@4.0.0-alpha.2```
> **To use Bootstrap 4 styles: **
	>Run this in your terminal or secure shell:
	> >npm install --save bootstrap@4.0.0-alpha.2
		meteor add fourseven:scss
		
>Create a main.scss in any place in client folder like client/styles/main.scss.
	Inside of main.scss, write
	> >@import "{}/node_modules/bootstrap/scss/bootstrap.scss";
	
>on top
### Git
##### Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
 ``` create a new repository  ```
 > **basic usage**
 >  ```git init ``` ----- to create a new git repository.
 
 ``` checkout a repository  ```
 > **basic usage**
 >  ```git clone /path/to/repository``` ----- create a working copy of a local repository by running the command.
 >     ```git clone username@host:/path/to/repository``` ----- when using a remote server.

 ``` add & commit  ```
 > **basic usage**
 >  ```git add <filename>``` or ```git add *``` ----- You can propose changes (add it to the Index) using this.
 >     ```git commit -m "Commit message"``` ----- To actually commit these changes

 ``` pushing changes  ```
 > **basic usage**
 >  ```git push origin master``` ----- To send those changes to your remote repository
 >     ```git remote add origin <server>``` ----- If you have not cloned an existing repository and want to connect your repository to a remote server,
  
   ``` branching  ```
 > **basic usage**
 >  ```git checkout -b feature_x``` ----- create a new branch named "feature_x" and switch to it using
 >     ```git checkout master``` ----- switch back to master
 >      ```git branch -d feature_x``` ----- and delete the branch again
 >      ```git push origin <branch>``` ----- a branch is not available to others unless you push the branch to your remote repository

update & merge
 > **basic usage**
 >  ```git pull``` ----- to update your local repository to the newest commit
 >     ```git merge <branch>``` ----- sto merge another branch into your active branch (e.g. master)
 >      ```git add <filename>``` ----- After changing, you need to mark them as merged 
 >      ```git diff <source_branch> <target_branch>``` ----- before merging changes, you can also preview them

log
 > **basic usage**
 >  ```git log``` ----- you can study repository history
 >     ```git log --help``` ----- These are just a few of the possible parameters you can use. For more
 

**Workflow:**  ``` your local repository consists of three "trees" maintained by git  ```

1. ``` Working Directory  ```  ----  which holds the actual files
2.  ``` Index ```  which acts as a staging area
3.  ``` HEAD ```  which points to the last commit you've made



  

