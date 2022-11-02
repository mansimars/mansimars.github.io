Host an online resume and README
==================================

## Purpose
------------
Learning how to host and format a resume using the software stack. We will use Markdown, a Markdown editor, GitHub pages, and Jekyll to achieve the purpose.

We will also learn the general principles of current Technical Writing, as explained in Andrew Etter's book _Modern Technical Writing_.

## Prerequisites
-----------------
* **Markdown knowledge**: You need to know how to use markdown. Don't know how to use Markdown? Check for Markdown tutorial under "More Resources".
* **Resume:** You need to have an updated resume formatted in Markdown format. My sample Markdown formatted [resume]() can be found here.
* **Github Profile**: You need to have a GitHub profile so that you can have upload your code and have the updated version of your files. Don't have a GitHub account? You can [sign-up](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) for the GitHub account here.

## Instructions 
-----------------
### **Markdown: Lightweight Markup Language**
>   Markdown is one of the best Lightweight markup language as it has the cleanest syntax incredible and infuriating, wonderful and maddening. Markdown does not have any defined standard and has limited set of features.[^1]
>
> For more broad compatibility, we can use "vanilla" Markdown syntax but we cannot use the tables and denced code blocks in vanilla Markdown syntax. We can also change to a different flavour but we would need to make some changes to source files according to the new flavour.[^2]

### **Use Distributed Version Control** 
> Distributed version control system (DVCS) allows us to work offline and have comparatively better performance. It also helps to work concurrently on the same set of files. All developers prefer using DVCS so it would be beneficial for the technical writers to use distributed version control system to work on documentations.[^3]
>
> In addition to that, we do not need to to use ```git reflog``` if we are using DVCS for documentation purposes. 
>
> There are some benefits of storing documentation in the same repository of the souce code.[^4]
> * The code and the documentation branches stay in sync.
> * New developers have more probability to contribute as new developers do not need to clone a separate repository.
1. Go to [GitHub](https://github.com/) and create a new repository by clicking on *New* from the top-left of the screen.
2. Name your repository as ```your-github-name.github.io```. 
    * For example: I created mine as ```mansimars.github.io```.
3. Make sure you select the repository as *Public* so that you can everyone can view your website.
4. You can either clone the repository to your local machine so that you can make the changes directly to GitHub repository or can upload your updated resume directly.
    * To clone repository from your local machine:         
      1. Click on *Code* which is located in top-right of the github repository and copy the link.
      2. Then install git on your local machine from this [link](https://git-scm.com/downloads). 
      3. Once the git is installed, open *Git Bash*.
      4. Clone the repository by typing ```git clone [link]```.
      5. Create your resume/file in your local machine in the same folder of your repository.
      6. Add your file using ```git add .```
      7. Commit changes using ```git commit -m "[your message]```".
      8. Upload your changes to GitHub repository using ```git push```.
   * To upload the file directly to GitHub repository:
     1. Click on _uploading an existing file_
     2. Choose your resume/file from your local machine.
     3. Click on _commit changes_.


### **Make Static Websites**
> Static websites are simple, secure, fast and portable. Static websites does not have server-side application dependencies so need to rely to databases and don't need to install anything. Thus, we can migrate the entire websites easily. We can also host it on Amazon S3 and Github Pages.[^5]
>
> Not only that, we can test the static websites on our local machine without installing anything. Static websites are secure as there is nothing to crash if someone tries to hack it.[^5]
>
> We can use generators to make complex websites. We need to provide with content and a theme to make a complex website. [^5]
1. **Install Ruby**  \
Download and Install Ruby to your local machine using this [link](https://www.ruby-lang.org/en/documentation/installation/). \
You can install the specific Ruby installer depending on the operating system.

2. **Install Jekyll** \
Once the Ruby is installed, install Jekyll by typing ```gem install jekyll bundler```. \
You can also get more detailed Jekyll installation steps by following this [link](https://jekyllrb.com/docs/). 

3. **Create Jekyll site** \
Type the following commands in the command prompt:
   1. Create Jekyll site: ```jekyll new [myblog]``` in your repository folder,
   2. Change to the specific directory: ```cd [myblog]```
   3.  Building and making a site available on local server: ``` bundle exec jekyll serve```
   4. You can check the website at [http://localhost:4000](http://localhost:4000)


4. **Publish your resume/file** \
To view your own resume/file, please follow the steps below:
   1. Rename your resume/file to index.md.
   2. Edit your index.md and add the command mentioned below at the top of index.md.
      *  Also Change the date and time to current date and time in the command below.
      ```yml
                ---
                layout: home
                title:  "Resume"
                date:   2022-11-01 15:02:18 -0500
                categories: jekyll update
                ---
      ```  
   3. Save changes and push it to the GitHub.  
   4. You can view your published website by going ```https://[github-name].github.io``` 

![Resume](/giffy.gif)
#### **More Resources**
1. [Markdown Tutorial](https://learnxinyminutes.com/docs/markdown/)
2. [Etter's Book](https://www.goodreads.com/author/show/14827025.Andrew_Etter)
3. [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf) 

## Authors and Acknowledgements
---------------------------------
The author of this README.md is [Mansimar Singh](https://github.com/mansimars).

I want to thank my group member of course COMP 3040 who reviewed my README file and helped me understand the concepts of Technical Communication.

1. Josh Sigurdson
2. Vedant Pulahru
3. Taylor Roy


## FAQs
---------
Why is Markdown better than a word
processor?
> Markdown is better than a word as it gives more freedom to the user to convert it to another files such as pdf, docx, html and then can be used anywhere depending on the specifications. In addition to that, we do not need to keep other formatted files as we can convert it anytime we need it. 

Can I use any other static site generator? Can you recommend some? 
> Yes, you can use other static site generators. Hugo, Gridsome, Eleventy, Pelican are also good static site generator that can help you to host a profile.

[^1]: Andrew Etter's *Modern Technical Writing*., p. 20
[^2]: Andrew Etter's *Modern Technical Writing*., p. 21
[^3]: Andrew Etter's *Modern Technical Writing*., p. 23
[^4]: Andrew Etter's *Modern Technical Writing*., p. 24
[^5]: Andrew Etter's *Modern Technical Writing*., p. 26
[^6]: Andrew Etter's *Modern Technical Writing*., p. 33