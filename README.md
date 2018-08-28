# My Journey - Fitness App

Link to App: [https://cdt12988.github.io/fitness-app/](https://cdt12988.github.io/fitness-app/ “My Journey”)

Ready to start your fitness journey?  The My Journey app is a tool designed to help you along the way!  Just create an account, choose your goals, and start logging your daily activities.

## App Features

### User Authentication

The My Journey app uses Firebase for multiple purposes, including user authentication.  The app allows new users to sign up with a username, email address, and password.  An email verification is then sent to the provided email address and the user is redirected to the home page.  Users can perform all the tasks you would expect of a complete login system, including resetting their password.  The app detects if users are signed in or not and refuses access to its contents to anyone not properly signed in.

### Tutorial Program

Once a user has signed up for My Journey, the app detects if it is their first time ever logging in.  If it is, it will then run a quick tutorial program designed to gather goals and information from the user and calculate default nutritional info based on the data the user gave.  The tutorial can be skipped and revisited later if desired.

### Home Page

After running the tutorial program and any time, thereafter, the user logs in, they are taken to the home page which will display the current daily progress of their goals.  This data is updated in real time.  So, after every single log entered by the user, their progress will display accordingly on the home page.

From this page, the user can access the two main features of the app: the Nutrition and Workout menus.  (The workout menu is still under development and not yet functional.)

### Nutrition

The nutrition menu is where all nutritional information is displayed and logged.  The landing page will display the user’s daily nutritional logs.  This will default to the current day, but users can also click through and view logs from previous days.  Users can add food to their daily log in a variety of ways.

#### Search for Food

Users can search for specific foods stored within the USDA Nutritional Database.  The search can include name brand products, or name brands can be excluded to yield better search results for more generic items, such as produce.

The search results display the nutritional information for the food per 100g of the food, but once selected, the user can choose a specific serving size and amount to add to their daily log.  The nutritional data is updated in real time so the user knows how many calories and other nutrients will be added to their log before they click to add it.

#### Quick Add

If the user can’t find what they are looking for via their search, or if they want to add a custom food to their log, they can use the quick add feature which allows them to input the name of the food and its nutritional value manually and add it to their daily log.

### Saved Foods

Users have the option to save particular foods that they would like to quickly access later.  Saved foods can be found under the “Saved” tab where they can then be added to the user’s daily log, if desired.

### Recent Foods

All recently added foods show up in the “Recent” tab.  Currently, the user can only add recent foods to their saved food, but adding directly to the user’s daily log from this menu is a feature that can also be added in the future.

### Frequent Foods

In addition to the most recent foods, the user can also view their most frequently logged foods within the “Frequent” tab.  Like the recent foods, frequent foods can only be added to the user’s saved foods, currently.  Though, this also can be changed in the future.

### Workouts

The workout menu was unable to be completed in the allotted time for this project, but is something that could definitely be added in the future to improve the utility of the app.

### Data Storage

Upon signing up, users are given a unique id which allows the app to track who is signed in and to access their specific records from the database.  This ensures that multiple users can be signed into the app at the same time, and only their own information is displayed back to them.  The app stores user information entered into the app, user nutritional information and goals, and daily log entries added by the user.

## Development Notes

### Languages, Frameworks, and Tools Used

* HTML5
* CSS3
* JavaScript
* jQuery
* Moment.JS
* Bootstrap
* Firebase (Database Storage and User Authentication)
* USDA Food and Nutrition APIs (JSON formatting and Ajax calls)

### Contributors

* Cody Thompson ([https://github.com/cdt12988](https://github.com/cdt12988 “Cody’s Github”)
* Peter Jarrard ([https://github.com/PeterJ330](https://github.com/PeterJ330 “Peter’s Github”)
* Sadegh Sachedina ([https://github.com/sadeghsachedina](https://github.com/sadeghsachedina “Sadegh’s Github”)

### Desired Features

This app was made as part of a group project.  Unfortunately, we ran out of time to develop many of the features and minor quality of life improvements that we had intended to.  Below are some of these features.

* Fully functional and integrated Workout section
* Improved layout
* Mobile responsive
* Better Goal Tracking
* More user-friendly interface and functionality. Specifically:
	- The ability to edit/delete daily log entries
	- The ability to choose to either save foods or log them as a daily entry
	- The ability to select size and quantity amounts for all foods entered (not just through the search feature)
		- This would require refactoring how some of the foods are stored into and displayed from the database
* User profile where user information can be seen and edited
* Social media user authentication
	- Along with this, the ability to link social media accounts to previously authenticated accounts