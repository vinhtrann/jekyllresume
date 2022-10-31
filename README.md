# Host resume on Github Pages

### [Demo Website](https://vinhtrann.github.io/jekyllresume/)

A simple jekyll setup to host a markdown resume on Github Pages

# Prerequisites
- A resume formatted in markdown
    - If you are unsure on how to create a resume formatted in markdown, there is a resource linked below detailing how  
- A Github account
    - If you do not have an account yet, you can create one [here](https://github.com/join)  
- Ruby installed
    - Check by running ``` ruby -v ``` in a terminal or by checking if it is installed
- Jekyll installed
    - Check by running ``` jekyll -v ``` in a terminal or by checking if it is installed
- Git installed and linked to your github account
    - Check by running ``` git --version ``` in a terminal or by checking if it is installed
    - [Link your account](https://kbroman.org/github_tutorial/pages/first_time.html)  
- A Text Editor
    - Recommendation: [Notepad++](https://notepad-plus-plus.org/)

# Instructions
#### Fork the repository  
 1. Press the Fork button at the top right of the webpage  
     - This will create a separate version of the repository that will be attached to your github account. It will have its own history separate from any other repository  
 ![image](https://user-images.githubusercontent.com/64811274/199124259-1d521c41-10a9-4a91-8fd7-26c7c3b5288b.png)
 2. Modify the repository name and description as you see fit
 ![image](https://user-images.githubusercontent.com/64811274/198891396-a3870ab6-3034-438d-aec9-4a720fae87e5.png)
      - There should be a new repository created and listed under the github account that forked the repository
      - This step relates to the concept of cataloging the difference from Etter's Book. By using distributed version control and creating a repository, a log of all the changes made to the resume will be recorded. Instead of storing multiple copies of your resume with timestamps, you could look into the past to view an old version of the resume.
 
#### Clone the repository
 3. Open a terminal  
       - Windows and MacOS both come with a terminal pre-installed
       - Command prompt for Windows, and the Terminal app on MacOS
 4. Navigate to the directory where you want the repository saved
       - Directory navigation is platform dependent  
       - Saving the repository where the terminal opens (the root) is possible, but not recommended  
       - If you are unsure on how to use command line to navigate through the file structure, there are additional resources below for both MacOS and Windows
 5. Clone the repository by entering the command below, modified for your own personal repository
       - This will create a local copy of the repository on your machine. Any changes here will not reflect the repository on Github until the changes are committed and pushed
       
 
 ```
 git clone https://github.com/[GITHUB USERNAME]/[REPOSITORY NAME].git
 ```
 For example
 ```
 git clone https://github.com/vinhtrann/jekyllresume.git
 ```  
 
- If you are unsure on what link to clone, it is also available from the code dropdown in the repository on github pictured below:  
![image](https://user-images.githubusercontent.com/64811274/199119785-e31cf771-f1fc-43eb-8c6d-296e5d1dc102.png)  
![image](https://user-images.githubusercontent.com/64811274/199119455-05c9bfd3-976b-4d15-9d2e-efaf2de2c699.png)

 
 #### Insert the markdown formatted resume into the local repository
  6. Delete index.md from the root directory
      - The default index is a copy of a sample resume
  7. Place the resume in the root directory
  8. Rename the resume to index.md
  
  Example:  
  ![replaceFile](https://user-images.githubusercontent.com/64811274/199120522-d4def88f-4f8d-42c3-be38-5e54377d114e.gif)

  
  
  9. Modify index.md to include the following front matter block at the beginning of the file
  
  ```
  ---
  layout: resume
  ---
  ```
   Example:  
  ![image](https://user-images.githubusercontent.com/64811274/198893506-a2e58448-945e-4622-9ad5-e3d50145fffd.png)  
  
   10. Save the changes to the file

  #### Build the static site using jekyll  
   11. Enter the following command into the command line
       - This will generate the static web pages
   ```
   bundle exec jekyll build
   ```
  
  
  #### Commit and push the change
   12. Add the modified index file through the command line by with the following command
   ```
   git add .
   ```
   13. Commit the change
        - This will act as an entry in the changelog
        - The commit message will show in the logs alongside any changes to the resume. 
   ```
   git commit -m "[COMMIT MESSAGE]"
   ```
   14. Push the change to the remote repository
        - This will sync the changes made in the local repository to the remote repository hosted on github  
   ```
   git push
   ```
  
  #### Setup github pages
   15. Navigate to the settings tab from the forked repository on github
       - This is located towards the top of the web page, just under the github user and repository name.
   ![image](https://user-images.githubusercontent.com/64811274/199122957-6fef3ca9-6ea8-47d9-8452-3edc1b02f6ed.png)
   16. Navigate to pages on the left  
       - Located under the code and automation section  
   ![image](https://user-images.githubusercontent.com/64811274/199123099-a9691edd-4b6f-4659-9b79-5556081a95bd.png)  
   17. Select the main branch and hit save
   ![image](https://user-images.githubusercontent.com/64811274/199123177-fe79ed30-96c8-4fae-b851-76c78d9b8229.png)
       - The site will now be accessible from https://[Github username].github.io/[repositoryname]   
   Example: https://vinhtrann.github.io/jekyllresume/
       - This step relates to the concept and benefits of building a website from Etter's book. By hosting a resume online, this will guarantee that anyone viewing it will have the most up to date version. If you instead distributed pdf copies of your resume, those copies will grow stale with time and potential employers will have out of date information.
       
## Example of accessing the newly created web page
![Example](https://user-images.githubusercontent.com/64811274/199114849-3cae2c4c-1d05-4674-8a57-0fa7fad86155.gif)

# More Resources
[Markdown Tutorial](https://www.markdowntutorial.com/)  
[Command line file navigation (Windows)](https://blogs.umass.edu/Techbytes/2014/11/14/file-navigation-with-windows-command-prompt/)  
[Command line file navigation (MacOS)](https://www.macworld.com/article/221277/command-line-navigating-files-folders-mac-terminal.html)  
[Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)  
[Jekyll Installation](https://jekyllrb.com/docs/installation/)  
[Git Installation](https://docs.github.com/en/get-started/quickstart/set-up-git)  
[Ruby Installation](https://www.ruby-lang.org/en/documentation/installation/)  


# Authors and Acknowledgements
- Vinh Tran - Main Author
- Stewart Wilcox - For reviewing this document
- [Casual Writer](https://github.com/casualwriter/casual-markdown-cv) - For the resume styling


# FAQ
### "Why should I use Markdown over a word processor?"
Markdown is better than a word processor for multiple reasons. One reason is that markdown files work well with version control, whereas other formats such as Word's docx doesn't. Another eason is that it is possible to write markdown in plaintext. This eliminates the need for any specialized editor.

### "I have followed the instructions but the site returns a 404 error"
Wait a couple of minutes, github pages takes a few moments to setup the newly hosted website.

### "I failed to push the changes to the remote repository"
This is most likely due to not having authorization to push changes to your own remote repository. You can fix this by adding the correct credentials to your git config. [Instructions here](https://kbroman.org/github_tutorial/pages/first_time.html)

### "How do I change the resume's theme?"
Unfortunately there is only one theme in this repository. If you want to affect the styling of the resume, open the ```_layouts``` folder and modify ```resume.html```. This will require some basic HTML and CSS knowledge. For other pre-made styles visit [Casual Writer](https://github.com/casualwriter/casual-markdown-cv)
