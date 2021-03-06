# Third Milestone Project - Dishes

![mockup](static/img/mockup.PNG)

# Table Of Contents

1. UX
2. Features
3. Technologies Used
4. Testing
5. Deployment
6. Credits and Acknowledgements
7. Updates since the projects first submission

There are two goals for this website. The first is for external users to find and share recipes, the second is for the owners of the site to promote their brand of cooking utensils.

# UX

#### User Stories
- As an external user coming to the site I want the following:
    - When I land on the homepage I want to see the experiences that others have had.
    - I want to be able to easily sign into my account, or if I dont have an account I want ease in registering.
    - I want to be able to easily navigate throughout the website.
    - I want to be able to search for recipes that I am interested in.
    - I want to be able to add in my own recipes.

- As the owner of this webiste I want the following:
    - I want a positve first impression for when incoming users land on the site.
    - I want incoming users to be able to easily sign up or log in.
    - I want my brand of cooking utensils/tools to be promoted to incoming users.

#### Wireframes:
The five planes of UX were kept in mind from the beginning of the design to the end. However I deviated from the wireframes as I built out the wesite. In the beginning in making the wireframes I originally planned on having four screens. But as I continued to build out the website it became obvious that I would also need to include a profile page, a login,a register page and later on I was also inspired to add in a custom 404 page.

![Homepage](static/img/homepage.JPG)

![Gallery](static/img/gallery.JPG)

![Add](static/img/add.JPG)

![Homepage](static/img/search.JPG)

#### Design
The overall design for this website is simple but effective for the websites goals. The homepage instantly highlights a welcome message to a new user to join or for existing users to log in. Underneath that there is a carousel which slowly rotates through the brand of cooking utensils, upon clicking on an image the user is redirected to the utensils page which has greater information on the websites brand of cooking tools.

If the user wants to access the library of dishes/recipes, they either need to log in or register. Once they do this they will get access to their profile, the sites recipies from other users and they will be able to add/update/delete their own recipes and dishes on the website.

Throughout the website each form/table or center piece for that page is highlighted by a card panal which focuses the users attention. This provides for a good contrast between the background image and for a better user experience.

#### Styling 

The default font from materialize was kept as it seemed to provide a very easy to read style. -apple-system,BlinkMacSystemFont

#### Images

The background image was selected as it gave a perfect first impression for when a user first lands. It is instantly clear at first glance that this is a cooking related website.

The 3 previous user review images were also selected to give a great first impression, they show the wholesome dishes that have been created in the past from other users. 

The other images are the utensils. These were all selected to give a very clean and professional look. Thus promoting the brand Cookbook for the websites owners.

## Features
- Navbar at the top of each page which collapses into a side-nav provides easy navigation around the site.
- The homepage has a carousel that auto rotates through the cooking utensils to promote the owners brand.

    ![carousel](static/img/carosel.PNG)


- The profile page allows users to update or delete any previous recipies they have added. 
- There was an issue in updating the "type of dish" this has since been corrected.

    ![update](static/img/update_delete.PNG)

- The "Add Your Dish" page allows users to create and add their own dishes to the website.

    ![add](static/img/adddish.PNG)

- The "Dishes" page allows users to search all the recipies that have been added to the site.

    ![search](static/img/search.PNG)

- The "Join" page allows users to create their own registration details which are then stored on MongoDB and accessed once the user logs in.

    ![join](static/img/join.PNG)

    ![join](static/img/signin.PNG)

- A custom 404 page will give a friendly display to the user if they look for a page that isnt on the site.
    
    ![404](static/img/404page.PNG)
    
#### The data
For this project 3 collections were created inside the "dishes" database. They are "dish","dish_type" and "dish_users". I felt this was enough as it allowed for all the CRUD functionality that was necessary.

 - "dish_type" is a simple collection used as a choice for the users to select the type of dish they want when adding thier receipes.
 - "dish" calls upon "dish_type" for an input and has 3 additional inputs. One of these is "created_by", this allows for me to display only the relevent recipes to that particular users profile.
 - "dish_users" take the basic information of the user and uses "user_name" and "user_password" to verify the correct user logging in.


# Technologies Used

- HTML5 for the website strcuture.

- CSS3 for the websites appearence.

- Materialize

- JQuery

- Python3 for the backend

- MongoDB as a databasee

- Flask as a web framework

- Heroku and Github for deployment

# Testing

## Homepage
#### Desktop
Homepage works as intended on the desktop. 
The User lands on the page and everything displays correctly and the carousel of utensils rotates around as expected.
When the user clicks login in and enters the details they are redirected to thier profile page where they can see their details.
Currently when the user clicks to register they are redirected to the registration page, however upon submitting the form the registration page refreches. Will update this to redirect them to their profile

![deskhome](static/img/desktop.PNG)

#### Mobile
Homepage works as intended on the mobile. 
The User lands on the page and everything displays correctly and the carousel of utensils rotates around as expected.

![deskmobile](static/img/homemobile.PNG)

## Cooking Utensils
#### Desktop
Displayed as intended when it had place holder text. 
However once I added in a proper description the formatted grid of the desktop was thrown off. I have fixed this for the moment by taking out the l4 class in the columns.

![deskUtensils](static/img/utensilsdesk.PNG)

#### Mobile
Displays as intended except for the LOGO at the top, needs to be centered on the Navbar.
This has since been corrected with some CSS padding.

![mobileUtensils](static/img/utensilsmobile.PNG)

## Profile
#### Desktop
Table needs to be corrected, its currently extending out to the right. Can be fixed with a multiline text input field.

![deskprofile](static/img/profile.PNG)

#### Mobile
LOGO at the top needs to be centered on the Navbar. This has since been corrected with some CSS padding.
Table needs to be corrected, its currently extending out to the left. Can be fixed with a multiline text input field.

![mobileprofile](static/img/profilemobile.PNG)

## Dishes
#### Desktop
As on the Profile page the table on the Dishes page needs to be corrected. This has since been corrected by swapping out the input field with a textarea input and limiting it inside a container class.

![deskdishes](static/img/dishes.PNG)

#### Mobile
LOGO at the top needs to be centered on the Navbar. 
As on the Profile page the table on the Dishes page needs to be corrected.

![mobiledishes](static/img/dishesmobile.PNG)

Table needs to be corrected

## Add Your Dish

#### Desktop
The dishes page works as expected on the desktop. No need for any chages

![mobiledishes](static/img/add.PNG)

#### Desktop
The dishes page works as expected on the mobile. No need for any chages

![mobiledishes](static/img/addmobile.PNG)

## Custom 404 page

#### Desktop
The custom 404 page works as intended for the desktop

![404desktop](static/img/404page.PNG)

#### Mobile
The custom 404 page works as intended for the mobile

![404mobile](static/img/404mobile.PNG)

#### Testing On Different Devices:
1. 24 inche dell monitor
2. 16 inche lenovo laptop
3. Galaxy S5
4. Pixel 2
5. iPhone 6/7 & 8
6. iPhone X 
7. iPad
8. Galaxy Fold

#### Testing with the HTML, CSS, Javascript and Python Validators

All four validators were passed. The only issue was on Javascript validator where it was picking up the $ from the JQuery.

![html](static/img/htmlvalidator.PNG)

![html](static/img/cssvalidator.PNG)

![html](static/img/jsvalidator.PNG)

![html](static/img/pythonvalidator.PNG)

## Deployment

To deploy this project Heroku is needed for the backend, Github was used as a repository with HTML/CSS for the frontend and MongoDB to be used as a database. Accounts will be needed on these before starting. It is important to note that this project wont run locally unless the enviroment variables are set up correctly within the env.py file. These variables and values must be the same within the Heroku deployment tab.

#### Steps I took to deploy my project:
 - Start with the developement enviroment, in my case Gitpod
 - In the developement enviroment I installed the requirements for this project found in requirements.txt using the pip3 command.
 - I setup the database MongoDB. From there I set up the collections which I used to store users,dish types and dishes added by users.
 - The values of the collections in MongoDB is what stores the information displayed on the site.
    -   For example the dish_type collection I have currently has the values "Chinese","Thai","Indian","Mexican","Irish","Other"
 - I then choose a connection method and connected by following the instructions MongoDB provides once clicking "connect" on the collection.
 - Once this is done enviroment variables were needed. 
 - The enviroment vairables I used here are: "IP", "PORT", ""SECRET_KEY", "MONGO_URI", "MONGO_DBNAME"
 - I stored the enviroment variables in a file called "env.py" and then place that file in a ".gitignore" file. This ensured the enviroment variables are not pushed to Github for security reasons.
 - Once this was done the python file called "app.py" could be created and run by typing "python3 app.py" into the terminal.
 - Deployed the app on Github.
 - In the terminal the commands: "pip3 freeze --local > requirements.txt" and "echo web: python app.py > Procfile" told Heroku the dependencies and which file runs the app.
 - Then over in Heroku, I selected "Create new app"  (The app name must be unique)
 - I connected the app on Heroku to Github by selecting the deployment method in the deploy tab to Github, search the repository name and clicked connect.
 - I Made sure that the app had been deployed on Github so that updates on Github flowed into Heroku, otherwise there would be differences between them.
 - Once this was done the enviroment variables that were entered into the "env.py" file needed to be entered into Heroku into the "Config Vars" in the settings tab. 
 - Finally I ensured that automatic deployments were selected in the Deploy tab on Heroku so that changes flowed through.

#### Steps necessary for another user to deploy:
- From your chosen developement enviroment
- Install the requirements for this project found in the requirements.txt file
- MongoDB will be needed for a database
    - Create an account with Mongo
    - Create the clusters for users,dish types and dishes
    - The values of these clusters will be the data that feeds into the site
- Enviroment variables will be needed in the developement enviroment
    - Create an env.py file 
    - Create a gitignore file and type "env.py" into that file to hide your enviroment variables
    - Within the env.py this is where you can put your enviroment varialbes like I have above ("IP", "PORT", ""SECRET_KEY", "MONGO_URI", "MONGO_DBNAME")
- Make a Procfile and a requirements file so Heroku knows the main app and whats needed to run the app with "pip3 freeze --local > requirements.txt" and "echo web: python app.py > Procfile"
- Over in Heroku setup an account and create an app with a unique name
- Deploy your app on Github and then over on Heroku connect your Github repository within the deploy tab
- Within Config Vars on Heroku place your enviroment variables that are stored in your env.py file. (They must be exact)
- Make sure you push the requirements and the Procfile (git add requirements.txt, git add Procfile, git commit -m "adding requirements and Procfile, git push)
- Make sure you enable automatic deployment within the deploy tab on Heroku so that there are no differences between Gitub and Heroku
- You will now be able to find the app URL and open the app in the top oright hand corner

#### How to clone and deploy this project:
- Navigate to the repository where the project is stored.
- Click on the Code button which will give the option to download the content and the url.
- Copy the url.
- In your chosen IDE in the terminal type "git clone (followed by the copied url)".

#### How to Fork this project:
- Log onto github and at the top of this repository there is an option "Fork"
- This will give you a copy of the repository

Credits

- Materilize was used for the navbar, card panels and grid structure https://materializecss.com/
- Fontawesome was used for the icons in the site https://fontawesome.com/
- MongoDB was used as the database for the users CRUD operations https://cloud.mongodb.com/
- The enviroment variables that were used in this project were taken from the Code Institutes walkthrough project PythonMiniProject https://learn.codeinstitute.net/courses/course-v1:CodeInstitute+DCP101+2017_T3/courseware/9e2f12f5584e48acb3c29e9b0d7cc4fe/579bbf01edaf47938e6a860b8f08f275/
- Help on fixing my textarea was taken from Stackoverflow https://stackoverflow.com/questions/5271782/how-to-disable-the-resize-grabber-of-textarea

 The images used throughout the site were taken from the below links:
- https://pixnio.com/media/woman-cooking-breakfast-people-ingredients
- https://www.pxfuel.com/en/free-photo-eleiv
- https://www.wallpaperflare.com/cooked-dish-on-white-plate-flat-lay-photography-of-cooked-food-with-coffees-wallpaper-zuewu

- https://www.flickr.com/photos/30478819@N08/49576980893
- https://www.pinterest.ie/pin/490610953162756931/
- https://commons.wikimedia.org/wiki/File:Bengali_cooking_tools.JPG
- http://www.freeimageslive.co.uk/taxonomy/term/14/links.htm?page=4
- https://www.pxfuel.com/en/free-photo-eufmw
- https://www.indiamart.com/proddetail/kitchen-knife-set-17250618055.html
- https://pxhere.com/en/photo/894960
- https://www.pxfuel.com/en/free-photo-erzod
- https://www.piqsels.com/en/public-domain-photo-ftvfv

 Recipies and dishes that were added to the site were taken from the below:
- https://www.bbcgoodfood.com/recipes/thai-fried-prawn-pineapple-rice 
- https://www.bbcgoodfood.com/recipes/chicken-pad-thai
- https://www.bbcgoodfood.com/recipes/slow-cooked-irish-stew
- https://www.bbcgoodfood.com/recipes/irish-coddled-pork-cider
- https://www.bbcgoodfood.com/recipes/chinese-chicken-curry
- https://www.bbcgoodfood.com/recipes/mexican-bean-soup-guacamole


Acknowledgements
I was inspired to insert a custom 404 page thanks to this video https://www.youtube.com/watch?v=3O4ZmH5aolg


## Updates since the projects first submission
On the projects first submission attempt there were a few factors that caused it to fail these have been updated since.
They were criterion 1.3, criterion 1.6, criterion 3.1, criterion 4.3

For criterion 1.3 there was an issue when attempting to update dish on the form, the below code has been added which has resolved this

    {% for plate in dishes %}
        {% if dish.dish_type == plate.dish_type_name %}
            <option value="{{ plate.dish_type_name }}" selected>{{ plate.dish_type_name }} </option>
        {% else %}
            <option value="{{ plate.dish_type_name }}">{{ plate.dish_type_name }} </option>
        {% endif %}
    {% endfor %}


For criterion 1.6
There was an issue in passing the HTML validator which will be attached here before the project is resubmitted

Adding html validations for the pages below:

   ![home](static/img/validHTML_home.PNG)
   ![404](static/img/validHTML_404.PNG)
   ![login](static/img/validHTML_login.PNG)
   ![newdish](static/img/validHTML_newdish.PNG)
   ![register](static/img/validHTML_register.PNG)
   ![profile](static/img/validHTML_profile.PNG)
   ![updatedish](static/img/validHTML_home.PNG)
   ![utensils](static/img/validHTML_utensils.PNG)

criterion 3.1
There was an issue in some of the CRUD operations which have now all been amended with this code

    {% for plate in dishes %}
        {% if dish.dish_type == plate.dish_type_name %}
            <option value="{{ plate.dish_type_name }}" selected>{{ plate.dish_type_name }} </option>
        {% else %}
            <option value="{{ plate.dish_type_name }}">{{ plate.dish_type_name }} </option>
        {% endif %}
    {% endfor %}

criterion 4.3
Deployment process could be elaborated on further, I have since added more detail to the deployment process
