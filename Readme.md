# Castle Vapes

The purpose of this project is to create a website for a startup called Castle Vapes.
Castle Vapes is a company that sells bespoke,custom hand made vaping mods.
This site was built as my final milestone project for the Code Institute Full Stack Web Development diploma. 
## Demo

Live demo can be found [here](https://castle-vapes.herokuapp.com/)

## UX

### User stories
As a USER, I want to be able to:
- access the store from different devices
- search the store using keywords
- browse products by categories
- read more details about a product after clicking on it
- easily add or remove products to and from my shopping bag
- see my cart's total at any time 
- sort the list of available products
- create a profile
- edit my profile
- place an order
- receive confirmations of placed orders on my email

As a ADMIN I want to be able to:
- easily add, edit and delete products
- be able to control stock

### Strategy

My goal in the design was to create a simple,easy to navigate website with a white background,in order to highlight details/colours of products. 


### Skeleton
[Wireframes](https://github.com/misza80/CI_project4_CastleVapes/tree/master/Wireframes) 


### Surface
The typography was found on google fonts and I chose the font Great Vibes for logo and Montserrat for page's body.
I think these two fonts compliment each other well.
 
Colours used are whites and blacks only as not to distract users from product colours and details.
## Technologies

1.HTML\
2.CSS\
3.Materialize\
4.jQuery\
5.Flask\
6.Google Chrome Developer tools \
7.Django \
8.Heroku

## Features
This site uses collapsible navbar to manage the navigation list on smaller screens.


Features left to implement are to finish email notifications and implement stock control.
## Testing
I tested this project manually. \
Aim of the test was to verify that the webiste works correctly across different operating systems,browsers and devices.
Website was tested on Google Chrome,Firefox and Opera browsers in their latest versions.Website was tested on multiple mobile device (iPhone 5,6,XR Samsung Galaxy s5,Apple Ipad) to ensure compatibility and responsivness.
Chrome developer tools were also used to check for compatibility and responsiveness.
Collapsible navbar works correctly on mobile devices. 
Code was validated using W3C, JsHint and PEP8 online validation services.All links were tested manually and will open within same browser tab.I used a lot of console.log() to see if my code us running correctly.
#### Errors

Email notification functionality is not working,emails are not being sent out to activate accounts,confirm orders,etc.Was set up using gmail email account. Could not test with other vendors due to project submission deadline.

## Deployment

This site is hosted using Heroku, deployed directly from the Github master branch. The deployed site will update automatically upon new commits to the master branch.
In order to setup I did the following:

- **Created a new repository:**
  From the main page I clicked on "New repository" button,gave it a name and clicked "Create a repository" button.


- **VS Code Setup:**
  For writing code I've used VisualStudio Code (VS Code).
  To get VS Code working correctly with GitHub,you need to install latest version of Git first,after that you can install VS Code.
  When installation finished I have cloned my repository,first by copying to clipboard the link to repository from the github page and then pasting it after `git clone` command into VS Code terminal.
  After selecting the save folder, proceeded to creating files and folders for my project.
  From the source control tab I could stage and commit changes to the repository.
  After entering the commit message I was able to push the committed changes.
  
For the purpose of processing payments, stripe account was created during the development process.
Following card details can be used for making test purchases:

| Card number      | CVC        | Date   |ZIP|
| -----------------|:------------:| ------:|---:|
| 4242 4242 4242 4242   | any number | any future date |any number|

Before deployment I created a public S3 Bucket on Amazon Web Services (consult AWS's website for how to do this)
Downloaded the 'new_user_credentials.csv' to a safe place after creating the user.These credentials were later used in setting up variables in Heroku.

This project was then deployed to Heroku to host the live application, following the steps below:

1.Log in to Heroku and create a new app called 'castle-vapes'\
2.Added Heroku Postgres DB and migrated db 
3.Log in to Heroku in the CLI\
4.Add the remote Heroku repo\
5.Create the requirements.txt file by running pip3 freeze --local > requirements.txt in the CLI\
6.Create a Procfile by running echo web: python run.py > Procfile in the CLI\
7.Start a web process on Heroku by running heroku ps:scale web=1 in the CLI\
8.Set environment variables in Heroku for Stripe,AWS and Django secret keys\
Restart all dynos on Heroku


### Content

Images for vape mods were obtained from Google Images.

### Media

Front page video was mad from static images obtained from Google Images.

### Acknowledgements

Special thanks to Chris Zielinski for his continuous support on slack.

I received inspiration, and based the code for this project from Code Institute's 'Full Stack Frameworks With Django' course material.

Wireframes were made using www.moqups.com
 

**This is for educational use.**
