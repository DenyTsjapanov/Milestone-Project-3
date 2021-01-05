# Milestone Project 3 ("WANTiT!") 

Project is deployed with Heroku at: https://i-wanna-app.herokuapp.com/

"WANTiT!" is a basic wishlist app. It provides the function (under the CRUD method) to create, view, edit and/or delete items by user's input. A user can create an account, after which he can create items to be stored inside of the wishlist. These items are presented in a Bootstrap card form, providing basic information, such as tyhe item's name, optional description, price and a button that targets a link to an online webshop offering said item/product. Whilst logged in, the user can the view his/her profile to view all items, and subsequently edit or completely remove items from the account. When not logged it, all users have access to viewing all stored and uploaded items as part of the "Get ideas for a gift" understanding.
 
## UX
 
The most important part of this app is its simplicity. Upon loading of the app, the user is greeted with a bulk of items in card forms. These items can only be viewed, regardless of whether the user is logged in or not. This prevents any users that are not logged in to make any modifications, and user that are logged in to accidentally edit or delete entries.

Files to wireframes are [here](https://github.com/DenyTsjapanov/Milestone-Project-3/tree/master/wireframes)

## Features

Users can create an account, which is password protected (db in MongoDB is being updated with "users" each time an account is created. Once created, users can add items to their wishlist consisting of an item name, optional description, image and URL to the webshop that offers said item. Inside of users' profiles, users can edit and delete their entries. Going to the "home" page, users are presented with items created by all users. These items can only be viewed, even when logged in, to prevent accidental edits or removal. No existing users cannot create items without an account, but can browse items created by other users. 
 
### Existing Features
- Register: allowes new users to create an account and have access to creating (and editing and deleting) items;
- Login: allows existing users to log in to their account and view, edit and delete their own entries;
- Logout: allows user to clear session (session.pop) and log out of the system, leaving only the option to view all items created by all users in the home page.

When logged in:
- View: allows users to follow the link to the online store that offers the particular item/product;
- Edit: edit entries such as, item name, description, price, category, URL and image (also URL);
- Delete: allows users to delete items from their wishlist.


### Features Left to Implement
- Sharing items or user profiles with other (non)users to actually distribute the wishlist.

## Technologies Used

In this section, you should mention all of the languages, frameworks, libraries, and any other tools that you have used to construct this project. For each, provide its name, a link to its official site and a short sentence of why it was used.

- [JQuery](https://jquery.com)
    - This project uses jQuery especially for Bootstrap and AOS (animate on scroll);
- Python:
    - Flask is installed with Python to create back end app and manipulate HTML with template rendering and redirecting. Aso with Jinja to make references within html files
- JavaScript:
    - JS is used for back to top button to easliy navigate the user to the top of the page once the footer has been reached.
 - MongoDB:
     - MongoDB is used for creating and storing data, based on user input, both user accounts, as well as items.
 - HTML & CSS:
     - For structure and styling.


## Testing

Due to lack of time, testing was held to the minimum. All testing took place by means of trial and error. Using the console helped with issued that took place from Heroku. Heroku refused to load the collapsable navigation bar when viewing the pages in mobile (or tablet) view. Restarting heroku fixed this issue. 

Jinja was also very helpful is finding issues, as it provides indications in its error messages. 

## Deployment

Deployment too place with Heroku. Within Heroku, I created a new app, and added the information from the env.py file to make connections. Further, from GitPod terminal, I added the requirements.txt file, so that Heroku know which requirements this project has. Furthermore, the Procfile was created for web. 

Finally, Heroku app was linked to the GitHub repo and enabled deployment from GitHub. This was, each time that the project was pushed to GitHub, Heroku was automatically updated. 


## Credits

- My mentor Reuben Ferrante has always been very helpful in properly explaining what is expected from me, even when I had issues understanding the language or requirements.
- As usual, W3Schools are amazing for quickly looking up when you're stuck. This also goes for StackOverflow and CSSTricks. 
- Bootstrap provides a ton of useful information, and a year later I find myself constantly getting new information from simply reading a new section.
- My wife and friends, who have tested the app on different devices and provided me with feedback for user interface, user experience and bugs.

### Content & Media
- All content is originated from offical websites that offer the item/product for sale. This includes text, as well as images.
