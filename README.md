# Host resume on Github Pages

### [Demo Website](https://vinhtrann.github.io/jekyllresume/)

A simple jekyll setup to host a resume on Github Pages

# Prerequisites
- A resume formatted in markdown
- Ruby
- Jekyll
- Git
- A Text Editor
- A Github account

# Instructions
#### Fork the repository  
 1. Press the Fork button at the top right of the webpage  
 ![image](https://user-images.githubusercontent.com/64811274/198891278-2046a31e-f5c7-4b98-9d94-521b6467e07d.png)  
 2. Modify the settings as you see fit and create the new fork  
 ![image](https://user-images.githubusercontent.com/64811274/198891396-a3870ab6-3034-438d-aec9-4a720fae87e5.png)
 
#### Clone the repository
 3. Open a terminal (Command prompt for windows, Terminal for MacOS)
 4. Navigate to the directory where you want the repository saved
       - If you are unsure on how to navigate through the file structure there are additional resoruces below detailing how
 5. Clone the repository enter the command below, modified for your own personal repository
 
 ```
 git clone https://github.com/[GITHUB USERNAME]/[REPOSITORY NAME].git
 ```
 - For example:
 ```
 git clone https://github.com/vinhtrann/jekyllresume.git
 ```
 
 #### Insert the markdown formatted resume
  6. Delete index.md from the root directory
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
   ```
   bundle exec jekyll build
   ```
  
  
  #### Commit and push the change
   12. Add the modified index file with:
   ```
   git add .
   ```
   13. Commit the change
   ```
   git commit -m "[COMMIT MESSAGE]"
   ```
   14. Push the change to the remote repository
   ```
   git push
   ```
  
  #### Setup github pages
   15. Navigate to the settings tab from the main repository on github
   ![image](https://user-images.githubusercontent.com/64811274/198894207-3a2cb6d8-083d-4993-b321-a569966007f7.png)
   16. Navigate to pages on the left  
   ![image](https://user-images.githubusercontent.com/64811274/198894506-0bac759b-9755-4547-9e0f-ff46caf2aadb.png)  
   17. Select the main branch and hit save
   ![image](https://user-images.githubusercontent.com/64811274/198894543-927ad311-c589-4b0a-bb82-b26cc0e226af.png)
       - The site will now be accessible from https://[Github username].github.io/[repositoryname]   
   Example: https://vinhtrann.github.io/jekyllresume/


# More Resources
[Markdown Tutorial](https://www.markdowntutorial.com/)  
[Command line file navigation (Windows)](https://blogs.umass.edu/Techbytes/2014/11/14/file-navigation-with-windows-command-prompt/)  
[Command line file navigation (MacOS)](https://www.macworld.com/article/221277/command-line-navigating-files-folders-mac-terminal.html)  
[Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)  


# Authors and Acknowledgements
- Vinh Tran - Created the blank template
- Stuart - for reviewing this document


# FAQ
### "Why is Markdown better than a word processor?"
Markdown is better than a word processor for multiple reasons. One reason is that markdown files work well with version control, whereas other formats such as Word's docx doesn't. Another eason is that it is possible to write markdown in plaintext. This eliminates the need for any specialized editor.

### "I followed the instructions but the site doesn't have my resume"
Wait a couple of minutes, github pages takes a few moments to setup.
