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
1. Fork the repository  
 a. Press the Fork button at the top right of the webpage  
 ![image](https://user-images.githubusercontent.com/64811274/198891278-2046a31e-f5c7-4b98-9d94-521b6467e07d.png)  
 b. Modify the settings as you see fit and create the new fork  
 ![image](https://user-images.githubusercontent.com/64811274/198891396-a3870ab6-3034-438d-aec9-4a720fae87e5.png)
 
2. Clone the repository
 - Open a terminal (Command prompt for windows, Terminal for MacOS)
 - Navigate to the directory where you want the repository saved
   - If you are unsure on how to navigate through the file structure there are additional resoruces below detailing how
 - Clone the repository enter the command below, modified for your own personal repository
 
 ```
 git clone https://github.com/[GITHUB USERNAME]/[REPOSITORY NAME].git
 ```
 - For example:
 ```
 git clone https://github.com/vinhtrann/jekyllresume.git
 ```
 
 3. Insert the markdown formatted resume
  - Delete index.md from the root directory
  - Place the resume in the root directory
  - Rename the resume to index.md
  - Modify index.md to include the following front matter block at the beginning
  
  ```
  ---
  layout: resume
  ---
  ```
   Example:  
  ![image](https://user-images.githubusercontent.com/64811274/198893506-a2e58448-945e-4622-9ad5-e3d50145fffd.png)
  - Save the changes
  
  4. Commit the change
   - Add the modified index file with:
   ```
   git add .
   ```
   - Commit the change
   ```
   git commit -m "[COMMIT MESSAGE]"
   ```
   
  5. Push the change to the remote repository
  ```
  git push
  ```
  
  6. Setup github pages
   - 
  

  

 




# More Resources


# Authors and Acknowledgements


# FAQ

