## FoodLuv

# Table of Contents

- [UX](#ux)
- [Design](#design)
- [User Stories](#user-stories)
- [Wireframes](#wireframes)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Testing](#testing)
- [Deployment](#deployment)
- [Credits](#credits)

## This website was created as part of milestone 3 for the code institute covering off the Data Centric Module
This site was created using Python as the programming language, Flask as the Python micro-framework & MongoDB Atlas as the Database. It was finally deployed using Heroku.
  
 > [Live Site](http://abushell-foodluv.herokuapp.com/home)
  
  >[Repository](https://github.com/TheBigBushman/foodluv/tree/master)



## UX
***Overview***
The website itself was designed heavily off the back of the CI mini project. 

Vast amounts of the code used has been reaftored to suit my needs from the CI.

The purpose was to allow users to sign up to the site and add and refer to recipes. 

***Metrics***
The data metrics a user can add and/or edit include:
>Cuisine Name
>Recipe Name
>Ingredients
>Difficulty
>Time to Cook
>Preparation

The admin of the site has additional privileges to be able to manage cuisines on the site.

## Design

**Typography**
I have chosen to go with Satisfy & Cursive for this website.

Satisfy is used as the main content font for the entire website.

Cursive is used for the web logo.

**Imagery**
The images sourced for this project came from unsplash.com. The idea was to show interesting vibrant meals to attract users.




## User Stories



> As an owner want to be able to manage food database that will grow overtime with the input from users and expand the site to become an authority site where I can then add options to buyer to purchase suggested cooking tools.
> 
>**Jane is an avid cooker and likes to experiment with different recipe ideas and wants to be able to keep her idea online so she can refer back to them in a consistent place. |She wants the ability to be able to add her own content, update recipes as they change and remove them if they are not what she wants.**
>
> Dave is a student who does not really know much about cooking and is looking for inspiration from others. He wants to be able to sign up to a website and be able to find easy meals to cook that appeal to him. 
>
>**As a beginner on the website I want to be able to setup an account and view recipes with the option of adding my own in the future.**




## Wireframes



The wireframes for this project were designed using MockFlow. Initial concept allowed for rating system and more of a user friendly functionality but due to time constraints the end product was more basic with the option for more advanced features in the future.
Wireframe located  [Here](https://github.com/TheBigBushman/foodluv/blob/master/static/wireframes/MS3%20wireframe.pdf).

## Features


**Home Page**

Navigation bar with logo font to the left followed by 3 initial options: Home, Login, Register.

Once logged in user will be presented with: Add recipe, Recipes, Sign Out. Admin has permissions for manage cuisines.

 >**Home Page** - Background carousel as a center piece to attract user to the page. Stock images from unsplash.com showcasing different food dishes.
 
 >**Card Section** - 3 cards to show features and sign up button.

 >**Footer** - Footer element contains links to Sign Up, Login and Home. 

**Recipes Page**
>View created recipes and edit or delete recipes created by the user. Only recipes created by the user can be deleted to prevent malicious behavior.
>By clicking on the Bin Icon a user can delete a recipe completely. 
>By clicking on the edit notepad a user will be brought to the edit from that has retained the recipe details for the creator to make changes.

**Add Recipe Page**
>Allows users to add recipes from scratch. 
>Once user selects cuisine it will predefine an image based on the cuisine type. This is to combat the issue with not being able to upload images to MongoDB. I retain the images in my static files and when users select a cuisine it selects the image I associated with it.

**Cuisines Page** (Only available to Admin)
>Allows Admin to manage, delete and create new cuisines for users to select.

****
**Socials**

Included social icons that are links but do not lead to anywhere as there are not socials set up for the site. This can be arranged at a later time. 

## Features Left to Implement

 >Search Functionality to allow users to find specific recipes
 
 >Separate sections by meal type. (Breakfast, Lunch, Dinner etc

>Cooking items to sell to users either through an affiliate scheme or for the owner to sell themselves.

>Allow user to save recipe data to dashboard (profile page) 

>Allow for nutritional input and create statistics based on what the user is cooking or expected to have.

>More detailed sign-up including e-mail capture to allow for newsletter / follow up e-mails

>Integrated share functionality to allow users to share recipe directly


## Technologies Used

**

**HTML**

>Basic structure for a web site

**CSS**

>Required to style my HTML and Images

**[Python](https://www.python.org//)**

>Programming language used for this project

**[Flask](https://flask.palletsprojects.com/en/1.1.x/)**

>Micro Framework used for the templating and logic of this project

**[MongoDB](https://www.mongodb.com/)**

>Database used for this project

**[Heroku](https://dashboard.heroku.com)**

>Cloud platform service used to support programming languages and used to deploy this project

**[Mockflow](https://Mockflow.com/)**

>Used to develop wireframes for this project

**[MaterialiseCSS](https://materializecss.com/)**

>Provided useful components and layout features to create this website. 

**[Git](https://git-scm.com/) / [GitHub](https://github.com/)**

>Used for version control and storing website

**[Font Awesome](https://fontawesome.com/)**

>Used this for icons and favicons for the likes of socials

**[Google Fonts](https://fonts.google.com/)**

>Used google fonts to pick appropriate fonts for this recipe site. 

**[Jquery](https://jquery.com/)**

>Used Jquery to help with the manipulation of the website and to bring other effects to life. 

**[Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)**

>Used to create functionality and interactivity on my site and to implement API's


## Testing

**Testing phase 1**
>For this project I opted for manual testing to ensure the app worked as intended from a user perspective
--------
**Testing on Chrome on handset mobile**
| Test |Outcome  |
|--|--|
|App header links showing only Home, login and sign up when not signed in| Pass  |
|Footer and page links directing to correct route| Pass
|Sign up allowing user to create account|Pass|
|Attempted login with incorrect credentials|Fail  |
|Login & sign up redirect to profile  | Pass|
|Full links showing on login except cuisines|Pass|
|User follows link for add recipe and adds correctly |Pass |
|User attempts one character on each field and submit |Fail  |
|User able to edit their own recipes|Pass|
|User unable to delete other recipes not created by themselves |Pass  |
|User able to edit recipes not created by themselves |Pass  |
|User able logout and no longer have CRUD functionality |Pass  |
|App log in header & footer return to home page |Pass  |



------------
**Testing on Chrome on Desktop using 19" display**
| Test |Outcome  |
|--|--|
|App header links showing only Home, login and sign up when not signed in| Pass  |
|Footer and page links directing to correct route| Pass
|Sign up allowing user to create account|Pass|
|Attempted login with incorrect credentials|Fail  |
|Login & sign up redirect to profile  | Pass|
|Full links showing on login except cuisines|Pass|
|User follows link for add recipe and adds correctly |Pass |
|User attempts one character on each field and submit |Fail  |
|User able to edit their own recipes|Pass|
|User unable to delete other recipes not created by themselves |Pass  |
|User able to edit recipes not created by themselves |Pass  |
|User able logout and no longer have CRUD functionality |Pass  |
|App log in header & footer return to home page |Pass  |





------------
**Testing Phase 2**


>**Same test samples as above except using internet explorer on mobile handset**

| Test |Outcome  |
|--|--|
|App header links showing only Home, login and sign up when not signed in| Pass  |
|Footer and page links directing to correct route| Pass
|Sign up allowing user to create account|Pass|
|Attempted login with incorrect credentials|Fail  |
|Login & sign up redirect to profile  | Pass|
|Full links showing on login except cuisines|Pass|
|User follows link for add recipe and adds correctly |Pass |
|User attempts one character on each field and submit |Fail  |
|User able to edit their own recipes|Pass|
|User unable to delete other recipes not created by themselves |Pass  |
|User able to edit recipes not created by themselves |Pass  |
|User able logout and no longer have CRUD functionality |Pass  |
|App log in header & footer return to home page |Pass  |
-------------
>**Testing on Chrome on Desktop using 19" display**

| Test |Outcome  |
|--|--|
|App header links showing only Home, login and sign up when not signed in| Pass  |
|Footer and page links directing to correct route| Pass
|Sign up allowing user to create account|Pass|
|Attempted login with incorrect credentials|Fail  |
|Login & sign up redirect to profile  | Pass|
|Full links showing on login except cuisines|Pass|
|User follows link for add recipe and adds correctly |Pass |
|User attempts one character on each field and submit |Fail  |
|User able to edit their own recipes|Pass|
|User unable to delete other recipes not created by themselves |Pass  |
|User able to edit recipes not created by themselves |Pass  |
|User able logout and no longer have CRUD functionality |Pass  |
|App log in header & footer return to home page |Pass  |
----------------
>**Tested each individual webpage on [w3.org](https://validator.w3.org/).**

|Page|Result  |
|--|--|
|Base| Pass 
|Home|Pass |

>**Pep8 Compliance for Python code validation**
Checked via Pep8 online [here](http://pep8online.com/checkresult)

|Page|Result  |
|--|--|
|PEP8 Result| Pass 
 

------------------------

** Group Testing Phase **
>Group testing was set out as a series of tasks to 2 individuals using different devices and a combination of browsers. These tests are to show usability and functionality that new users are able to navigate the site with ease. 

>These tests are:

|Test|Pass %  |
|--|--|
| Create an account / login for FoodLuv | 100% |
| View the current recipes| 100% |
| Add your favorite recipe| 100% |
| Remove 1 ingredient from your recipe| 100% |
| Replace that ingredient with Salt| 100% |
| Delete your recipe| 100% |
| View the ingredients of the pasta italian dish created by AlanBushell| 100% |
| Try to edit this recipe| 0% |
| Log out of the App| 100% |


**

>Testing on GTmetrix.com showed the Home page has a speed score of A (92%), A fully load time of 1.6 seconds. Test server location: Vancouver, Canada using chrome.

>Google Developer PageSpeed Insights gave the home page a score of 90 (Green)
Issues presenting appear to be how the carousel images are hosted and the size of these images.

## **Bugs**

> Throughout development I encountered issues how the recipes where not displaying correctly in rows and some where showing incorrect sizing. This issue was fixed to improve website aesthetics and overall UX

> Had issue with initial development as I could not connect my env.py file. It persisted in giving me errors as the variables were incorrect. Once I worked with CI via chat the issue was made clear.

> Recipes did not display on all recipes section. I set a for loop but did not call the database from the app.py file. Once I realized this issue I rectified it and the recipes displayed

## Deployment


To deploy the project I followed these steps:

The website is hosted via  [GitHub](https://github.com/), with the source code being available on  [my repository](https://github.com/TheBigBushman/foodluv).

### Requirements

-   **Python3**  to run your application
-   **PIP**  to install all app requirements
-   **IDE**  of your choice -Gitpod was used for this project
-   **MongoDB Atlas**  account for database development

### How To Access It

-   In order to run this project locally you should follow these steps:
    
    1.  Click the green  _'clone or download'_  button in the  [GitHub repository](https://github.com/TheBigBushman/foodluv)  for the project.
        
    2.  Copy the link provided by clicking the  **clipboard button**  to the right of the link.
        
    3.  In your terminal, type  _**git clone**_, paste in the previously copied link, and hit return.
        
    4.  Create a file called ".flaskenv" and add the following:
        
        -   **FLASK_APP=run.py**
        -   **FLASK_ENV=development**
    5.  Install the required modules with the command  **pip -r requirements.txt**.
        
    6.  If you don't have it yet, create a free account on  [MongoDB](https://mongodb.com/)  and create a new Database called  **Database3**.
        
    7.  Then create the following collections in that Database:
        
        -   **Cuisine**
            
            -   **_id:**< ObjectId >
            -   **cuisine_name:**< string >

        -   **recipes**
            
            -   **_id:**< ObjectId >
            -   **cusine_name:**< string >
            -   **recipe_name:**< string >
            -   **preperation:**< string >
            -   **ingredients:**< string >
            -   **time_to_cook:**< string >
            -   **difficulty:**< string >
            -   **created_by:**< string >

        -   **users**
            
            -   **_id:**< ObjectId >
            -   **username:**< string >
            -   **password:**< string >
            -   **email:**< string >
    8.  You should now be able to run this application locally by typing  **flask run**.
        

### Deployment to Heroku

1.  Create a  **requirements.txt**  file by typing  **pip3 freeze --local > requirements.txt**  into the terminal line.
    
2.  Create a Procfile by typing  **echo web: python app.py > Procfile**.
    
3.  Add, commit and push these changes to Github.
    
4.  Navigate to the  [Heroku](https://heroku.com/).
    
5.  Create new app and give it a unique name.
    
6.  Choose the region that is closest to you.
    
7.  Go to the  **Deploy**  tab and choose  **Github**.
    
8.  Search for the correct repository and connect.
    
9.  Go to Heroku  **Settings**  and navigate to  **Config Vars**.
    
10.  Set the following:
    
    -   **IP = 0.0.0.0**
    -   **MONGO_DBNAME = [Name of MongoDB]**
    -   **MONGO_URI = mongodb+srv://:@<cluster_name>-qtxun.mongodb.net/<database_name>?retryWrites=true&w=majority**
    -   **PORT = 5000**
    -   **SECRET_KEY = [Secret key]**
11.  Go to the Deploy tab and  **Deploy Branch**, ensuring that the master branch is selected.

## Credits

[**Codepen.io**](codepen.io)

>Viewed some websites for inspiration as to what to build and how to implement them.

**Nishant Kumar (Mentor)**
>Nishant again has had amazing faith and provided excellent guidance. I am extremely grateful for his feedback and guidance throughout this project.

**[Code Institute](https://codeinstitute.net/)** 
>Amazing course, has provided me with clear direction in everything I have created so far. The trainers explain things in a great way and provide great resources to be able to further learn.

**[Stack Overflow](https://stackoverflow.com/)**
>I frequently used stack overflow as a lot of my errors throughout this development were questions and problems others have faced in the past. 

**[w3Schools](https://www.w3schools.com/)**

>Amazing library of full web framework components to pull from and assisted with understanding the structure of certain elements. 

## Content


[**Unsplash**](https://www.unsplash.com/search/concert/)
>All images from this site were taken from unsplash, a free open source site for sharing images.
-------------

## Acknowledgements


>Code Institute
>Nishant Kumar
>Unsplash
>Traversy Media
>Bootstrap Library
>Materialise CSS
>Steve Griffith
