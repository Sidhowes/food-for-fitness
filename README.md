## Code Institute Data Centric Development Milestone Project
# Food For Fitness

Food For Fitness is a online cookbook where users can find and share healthy fitness related recipes to enjoy, as well as edit recipes if the user feels they can improve upon an existing recipe or delete all 
together if they feel the recipe is not a good standard.

![site logo](https://res.cloudinary.com/dnk59j2my/image/upload/v1603819267/Add_a_heading_7_c6upic.jpg)

[Visit deployed site]

## Device Viewings



## UI/UX
### Project Goal
This Project is a milestone project for Code Institute Data Centric Development module. The criteria for this project is to create a website using the CRUD functionality: Create, Read, Update and delete.
I have created a online healthy recipe website that uses CRUD to target the fitness indusrty.


### User Stories
As a user I would like to:
* View all recipes on one page.
* Access the website on mulitple devices i.e mobile and desktop.
* Add my own recipe.
* Be able to see and read my recipe on the recipes page.
* Update/edit my recipe.
* Delete my recipe once I have used the recipe or do not want it anymore.
* Be able to click on the recipe and see further details on ingredients and instructions on how to make the recipe.
* Be able to easily navigate through the website without prior knowledge of the website.
* Be able to filter recipes per category.


## Wireframes








### Defensive Design
* All forms cannot be left empty and must be filled out.
* Forms give feedback if a option is left blank or the right syntax is not used.

## Features
### Existing Features
* Food For Fitness logo acts as home button.
* Nav links to navagate through ther website.
* Nav links at the footer of the website for quick use of navagating through the website.
* Social links located at the footer for quick access to: Facebook, Instagram, LinkedIn and Twitter.
* Index page main image with inspirational wording.
* Index page has few example featured recipes to check out.
* Recipe page ahs a filter option, to filter which category you would like to see.
* Recipes Shown in list show category and cook time.
* Single recipe shows full information on how to make and cook recipe including how long it should take.
* Add recipe and edit recipe forms have clear instructions and character limits for certain fields.
* Bootstrap input field validation.

### Future Features
* Sign up page.
* Log in page.
* Log out page.
* Profile page.

## Technologies used
#### Below is a list of the programming languages, technologies, frameworks and resources used for this website.

* HTML5
* CSS3
* Javascript 
    * jQuery
* Python 3.8.2
    * Flask
    * Jinja
    * Werkzeug security
* MongoDB and MongoDB Compass
* Bootstrap CDN
* Git & GitHub.com
* Heroku.com pages
* Markdown
* FontAwesome.com
* Google Fonts
* Canva: Design of main image
* Google Chrome Developer tools
* Firefox Developer tools
* Cloudinary.com: Download image from Canva through Cloudinary to Gitpod.
* Materialize - base project layout

## Testing
### Used multiple devices to test functionality and visual appeal:

* Iphone - Safari
    * Iphone 10
    * Iphone 11
* Ipad - Safari
    * Ipad pro
* Sony 15.6inch laptop - Chrome
* Windows Toshiba tablet/laptop - Chrome

### Manual testing

Continuously testing the functionality and visuals on a laptop, ipad and mobile after every change or code inputted.
Used force refresh to ensure everything was how I intended it to be.

1. Home page/Recipe page

* Test if navigation bar works correctly on phone, tablet and desktop browsers
* Test if page is responsive at all sizes
* Test footer social icon links (links open homepages in a new window)

2. Add 

* Test the add recipe form that it adds to the database.
* Test that the recipe shows up on website after adding.
* Test that the form has to be  entered correctly and if not gives guidance on how to syntax the form.

3. Edit 

* Test that the edit button brings you to the edit page.
* Test that once edited it corrrectly shows the new edit on the recipe detail page.
* Test that the form has to be  entered correctly and if not gives guidance on how to syntax the form.

4. Delete

* Test that once clicked on the delete button a modal appears to and asks "are you sure you want to delete this recipe."
* Test that once deleted recipe it is also deleted off the database.
* Test that once clicked delete and modal appears and you click cancel on the modal. It does not delete recipe and take s you back to the recipe detail.

5. Flash messages

* Test once added a recipe, a flash message appears.
* Test once edited a recipe, a flash message appears.
* Test once deleted a recipe, a flash message appears.

### Validators

* [W3Cschools css validator](https://jigsaw.w3.org/css-validator/validator) - Validate my css code to make sure there are no errors.
* [W3Cschools html validator](https://validator.w3.org/) - Validate my html code to make sure there are no errors.
* [beautifytools javascript validator](http://beautifytools.com/javascript-validator.php) - Validate my javascript code.

## Deployment

For this project we used Heroku to deploy the app. We also use MongoDB as the databse holder and then Gitpod as our IDE.

#### MongoDB

First created a env.py file. This will store sensitvie information and we will use .gitignore to ignore the file when pushing to our website.
```
touch env.py
```
Within this file we can link our Mongo database.
```
"MONGO_URI", "mongodb+serv://..."
```
#### Heroku

Firstly we need to set up files that Heroku needs to run the app.

These are the applications and dependencies to run the app.
```
pip3 freeze --local > requirements.txt
```
Next the Procfile is what heroku looks for to know which file runs the app and how to run it.
```
echo web: python app.py > Procfile
```

Once the files have been created. Log on or create an account with Heroku and create an app.
* The app name must be unique with no spaces and in lower case.
* Link that app to the GitHub repository by going to the "Deployment method".
* Once linked scroll down to "Connect to Github" and add your repository name and click search and then connect.
* In the Settings tab, add the corresponding Config Variables as present in local development:
```
IP 0.0.0.0
PORT 5000
SECRET_KEY FJHFJD7474...
MONGO_URI mongodb+serv://...
MONGO_DBNAME ("name of database")
```
* Now that the config variables are inserted but before deployment you must go back and git push the Procfile and Requirements.txt
to github.
```
git add -A
```
```
git commit -m "Add Procfile and requirements.txt"
```
```
git push
```

* Next enable deployment on heroku
* Deploy master branch
* Now that we have Deployed Branch Heroku will start buliding the app which takes 2 minute.
* Once bulit it will have a message "Your app was successfully deployed."
* Click view underneath the message to launch the app.
* The app is now deployed on heroku and whenever you push changes to github it will also be linked to the heroku app.

While working on the project you must change from debug=False to debug=True located on the last line of the app.py file.
You will then be able to run the app locally by typing python app.py or flask run.
Then before submitting project change it back to debug=False

## Credits

### Content

* [Nav](https://materializecss.com/navbar.html)
* [Side-nav](https://materializecss.com/navbar.html)
* [Dropdown](https://materializecss.com/dropdown.html)
* [form](https://materializecss.com/text-inputs.html)
* [Modal](https://materializecss.com/modals.html)
* [Image-card](https://materializecss.com/cards.html)
* [Footer](https://materializecss.com/footer.html)
* [Recipe instructions/ingredients](https://www.bbcgoodfood.com/recipes/peri-peri-chicken-pilaf)

### Media

Majority of the images used are from google images

* [Home page main image](https://res.cloudinary.com/dnk59j2my/image/upload/v1603819267/Add_a_heading_7_c6upic.jpg)
* [Recipes page main image](https://www.berkeleywellness.com/sites/default/files/field/image/iStock-919666108-2_field_img_intro_774_500.webp)
* [Featured recipes images](https://www.google.com/search?q=healthy+meal+dish&tbm=isch&ved=2ahUKEwikg9zam_vsAhWE8IUKHSZaA5IQ2-cCegQIABAA&oq=healthy+meal+dish&gs_lcp=CgNpbWcQAzICCAA6BAgAEEM6BQgAELEDOgcIABCxAxBDOgYIABAIEB5Qr9ylC1iFjKYLYMmOpgtoAHAAeACAAYcBiAHBCpIBBDE1LjKYAQCgAQGqAQtnd3Mtd2l6LWltZ8ABAQ&sclient=img&ei=NzqsX-SLNYThlwSmtI2QCQ&bih=625&biw=1366)

#### Icons

All icons used from font-awesome:
* [Title](https://fontawesome.com/icons/heading?style=solid)
* [Category](https://fontawesome.com/icons/folder-open?style=solid)
* [Description](https://fontawesome.com/icons/align-left?style=solid)
* [Image url](https://fontawesome.com/icons/image?style=regular)
* [Cook time](https://fontawesome.com/icons/clock?style=solid)
* [Ingredients](https://fontawesome.com/icons/align-left?style=solid)
* [Instructions](https://fontawesome.com/icons/align-left?style=solid)
* [Facebook](https://fontawesome.com/icons/facebook-square?style=brands)
* [Instagram](https://fontawesome.com/icons/instagram?style=brands)
* [Twitter](https://fontawesome.com/icons/twitter-square?style=brands)
* [LinkedIn](https://fontawesome.com/icons/linkedin?style=brands)

## Acknowlegements

* Ingredients and Instructions from [BBC goodfood](https://www.bbcgoodfood.com/)
* Help and guidance from my mentor _Akshat Grag_.
* Inspiration from [Fresh Fitness Food](https://www.freshfitnessfood.com/)






