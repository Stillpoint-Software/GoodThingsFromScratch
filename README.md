# Site information

This site is using the Mangila theme [link](https://jekyllthemes.io/theme/mangila-blog-jekyll-theme) and Sveltia-cms [Link](https://github.com/sveltia/sveltia-cms) for admin.

The site is being hosted on Netlify and source code is on Sillpoint Software's github 

### Deployment
Since the project is attached to netlify, deployment happens automatically when you push to Github.  There is no setup to do in GitHub.  Netlify handles this as soon as you attach a GitHub repository.

### Local Setup

1.  Install Ruby 3.0.0 [link](https://rubyinstaller.org/)
2.  Install Ruby Gems [link](https://rubygems.org/)
3.  Open the project in VS Code
4.  From the terminal, install Jekyll `gem install jekyll`
5.  From the terminal, run `bundle install`
6.  To run the site locally, run `bundle exec jekyll serve` 

### Setup Admin

1.  Add an `admin` folder
2.  See sveltia-cms for the config.yml and index.html files and how to set them up [link] (https://github.com/sveltia/sveltia-cms?tab=readme-ov-file#getting-started)
3. to run the admin, start the server and add `/admin` to the end of the url.  You can run the admin locally without any additional setup.
 

### Github Setup

1.  Add the source code to a github repository.
2.  In the Settings of the `Github` organization, go to `Oauth`
3.  Click on `New OAuth app`
4.  Enter an appplication name, homepage url and application description
5.  Under Authorization callback URL enter `https://api.netlify.com/auth/done` (This is specific to Netlify)
6.  Copy the ClientID and Secret, you will need this for netlify
7.  Under third-party access, click on `GitHub Apps`
8.  Click on `Configure` next to "Netlify"
9.  Netlify needs Read access to code and metadata and Read and write access to checks, etc
10. Scroll down to `Repository access`
11. Select the repository you want to give Netlify access to

### Netlify Setup

1. Login to Netlify
2. Click on "New site from Git"
3. Select `GitHub` under connect to Git provider
4. Pick a respository
5. Enter an `Environment Variable` as follows:  RUGY_VERSION   3.0.0
6. Click on Forms `Forms`
7. Click on `Enable form detection`
8. Under `Site configuration`, click on OAuth
   1. click on `Install provider`
   2. Enter the Github Client Id and Secret
   3. Under `Notifications`, click on Emails and webhooks
   4. Under `Form submission notificiations`, add an email address that will received all the contact information when submitted.


* * *

### Documentation

Before using the Mangila theme, please read the documentation under the documentation folder.

* * *

### Style Guide
See the styleguide.md under the _pages folder