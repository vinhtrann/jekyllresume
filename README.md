# Host resume on Github Pages

### [Demo Website](https://vinhtrann.github.io/jekyllresume/)

A simple jekyll setup to host a resume on Github Pages

# Prerequisites
- A resume formatted in markdown
- Ruby installed
    - Check by running ``` ruby -v ``` in a terminal
- Jekyll
    - Check by running ``` jekyll -v ``` in a terminal
- Git
    - Check by running ``` git --version ``` in a terminal
- A Text Editor
- A Github account

# Instructions
#### Fork the repository  
 1. Press the Fork button at the top right of the webpage  
     - This will create a separate version of the repository where it will have its own history  
 ![image](https://user-images.githubusercontent.com/64811274/198891278-2046a31e-f5c7-4b98-9d94-521b6467e07d.png)  
 2. Modify the settings as you see fit and create the new fork  
 ![image](https://user-images.githubusercontent.com/64811274/198891396-a3870ab6-3034-438d-aec9-4a720fae87e5.png)
      - You should have a new repository listed under your github account now  
      - This step relates to the concept of cataloging the difference from Etter's Book. By creating a repository, it creates a log of all the changes made to the resume. If you wanted to view the state of your resume 6 months ago, it would be possible thanks to version control.
 
#### Clone the repository
 3. Open a terminal  
       - Windows and MacOS both come with a terminal pre-installed
       - Command prompt for windows, and the Terminal app on MacOS
 4. Navigate to the directory where you want the repository saved
       - Directory navigation is platform dependent
       - If you are unsure on how to use command line to navigate through the file structure, there are additional resources below for both MacOS and Windows
 5. Clone the repository by entering the command below, modified for your own personal repository
       - This will create a local copy of the repository on your machine. Any changes here will not reflect the repository on Github until the changes are committed and pushed
       
 
 ```
 git clone https://github.com/[GITHUB USERNAME]/[REPOSITORY NAME].git
 ```
 - For example:
 ```
 git clone https://github.com/vinhtrann/jekyllresume.git
 ```
 
 #### Insert the markdown formatted resume
  6. Delete index.md from the root directory
      - The default index is a copy of a sample resume
  7. Place the resume in the root directory
  8. Rename the resume to index.md
  9. Modify index.md to include the following front matter block at the beginning
  
  ```
  ---
  layout: resume
  ---
  ```
   Example:  
  ![image](https://user-images.githubusercontent.com/64811274/198893506-a2e58448-945e-4622-9ad5-e3d50145fffd.png)
  10. Save the changes

  #### Build the static site using jekyll  
   11. Enter the following command into the command line
       - This will generate the static web pages
   ```
   bundle exec jekyll build
   ```
  
  
  #### Commit and push the change
   12. Add the modified index file with:
   ```
   git add .
   ```
   13. Commit the change
        - The commit message will show in the logs alongside any changes to the resume. 
   ```
   git commit -m "[COMMIT MESSAGE]"
   ```
   14. Push the change to the remote repository
   ```
   git push
   ```
  
  #### Setup github pages
   15. Navigate to the settings tab from the forked repository on github
       - This is located towards the top of the web page, just under the github user and repository name.
   ![image](https://user-images.githubusercontent.com/64811274/198894207-3a2cb6d8-083d-4993-b321-a569966007f7.png)
   16. Navigate to pages on the left  
       - Located under the code and automation section
   ![image](https://user-images.githubusercontent.com/64811274/198894506-0bac759b-9755-4547-9e0f-ff46caf2aadb.png)  
   17. Select the main branch and hit save
   ![image](https://user-images.githubusercontent.com/64811274/198894543-927ad311-c589-4b0a-bb82-b26cc0e226af.png)
       - The site will now be accessible from https://[Github username].github.io/[repositoryname]   
   Example: https://vinhtrann.github.io/jekyllresume/
       - This step relates to the concept and benefits of building a website from Etter's book. By hosting a resume online, this will guarantee that anyone viewing it will have the most up to date version versus if you distributed pdf copies of your resume. The pdf copies of the resume will eventually grow stale.
       
## Example of accessing the newly created web page
![Animation](https://user-images.githubusercontent.com/64811274/198899492-96a36722-e885-4bfc-9159-c599b0f8ec76.gif)



# More Resources
[Markdown Tutorial](https://www.markdowntutorial.com/)  
[Command line file navigation (Windows)](https://blogs.umass.edu/Techbytes/2014/11/14/file-navigation-with-windows-command-prompt/)  
[Command line file navigation (MacOS)](https://www.macworld.com/article/221277/command-line-navigating-files-folders-mac-terminal.html)  
[Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)  
[Jekyll Installation](https://jekyllrb.com/docs/installation/)  
[Git Installation](https://docs.github.com/en/get-started/quickstart/set-up-git)  
[Ruby Installation](https://www.ruby-lang.org/en/documentation/installation/)  


# Authors and Acknowledgements
- Vinh Tran - Created the blank template
- Stuart - for reviewing this document


# FAQ
### "Why is Markdown better than a word processor?"
Markdown is better than a word processor for multiple reasons. One reason is that markdown files work well with version control, whereas other formats such as Word's docx doesn't. Another eason is that it is possible to write markdown in plaintext. This eliminates the need for any specialized editor.

### "I followed the instructions but the site doesn't have my resume"
Wait a couple of minutes, github pages takes a few moments to setup.

