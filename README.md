## How to host and format a resume on GitHub Pages Using Markdown and Jekyll



### Overview
This tutorial will cover how to format a resume in Markdown, followed by hosting it with a supported theme. The software stack used here is Markdown, Ghostwriter - a Markdown editor, GitHub Pages, and Jekyll. More on each of these below.



### Prerequisites
* A markdown editor
* A resume written in Markdown, with the editor of your choice
* Check the More Resources section on how to write in Markdown
* A GitHub profile



### Instructions
**1. Install Ruby**
* Go to the list of Ruby Installers (https://rubyinstaller.org/downloads/) and select the latest version in the 'WITH DEVKIT' section.
* Accept the License Agreement
* Check 'Add Ruby executables to your PATH'
* Select all the options to ensure all the necessary components are installed
* Check the 'Run ridk install' option and click finish
* When the command prompt opens, enter the option that reads 'MSYS2 and MINGW development toolchain' and press enter

**2. Install Jekyll**
* Open a new command prompt window and install Jekyll and Bundler using 'gem install jekyll bundler'
* Check if Jekyll has been installed properly by entering 'jekyll -v' in the command prompt and the correct version should be the output

**3. Run a static site with Jekyll**
* Open a new command prompt window and navigate to the folder (possibly after creating one) you want to host the site in. You can do this using the 'cd' command.
* Enter 'jekyll new \<name of site>'

**4. Getting a Jekyll Resume Theme**
* Visit RubyGems (https://rubygems.org/) - you can select between a wide range of themes that fits your resume
* Search for 'Jekyll Resume Theme' and select one that you prefer
* Scroll down on the theme page and under the 'Links' section, click on 'Homepage' to view what the theme might look like and read more about it
* Read the instructions on the page you land to install the theme

**5. Run the Static Site With Your Theme**
* Open a new command prompt window
* Navigate using the 'cd' command to the folder where your static site is located
* Enter 'bundle install'
* Enter 'bundle exec jekyll serve'
* A link to your website should pop up. You can enter this into your browser of choice and a new webpage with your resume should load up

**6. Make a GitHub Account**
* Vist GitHub (https://github.com/)
* Sign up for an account or sign in if you already have one
* Click on the Repositories tab
* Select the green icon to make a new repository
* Set the name of the repository to be '\<username>.github.io'
* Create the repository

**7. Pushing your resume onto GitHub**
* Go to your repository that you just created and copy the shareable link. You can also do this by clicking on the clipboard icon to the right of the link
* Open a new command prompt window 
* Navigate to the folder that you want to host using the 'cd' command
* Enter 'git init' to create a local repository on your machine
* Enter 'git add .' to add all the files to the staging process
* Enter 'git commit -m "<any comments on the changes you've made>"'
* Enter 'git remote add origin \<paste the link you copied earlier>'
* Enter 'git push origin master' to make the changes live on GitHub Pages



### More Resources
* https://www.markdowntutorial.com/ (markdown tutorial)
* https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS (book)
* https://docs.github.com/en/get-started/quickstart/create-a-repo (first repo)



### Authors and Acknowledgements
* crispgm (https://github.com/crispgm/resume)
* Jacob Broggy
* Joseph Gonzales
* Gurdit Singh



### FAQs
* Why is Markdown better than a word processor?

	Markdown is better than a word processor since it provides more freedom to edit and format lines of text. With basic tags to bold or italicize text, as well as create hyperlinks and add images, there is a wider range of utility for any user

* Why is my resume not showing up?

	Your resume could not be showing up due to an outdated version of Ruby, which should 3.5.0 or higher. Otherwise, there could be other factors such as a theme for your resume that is not supported by GitHub Pages.
