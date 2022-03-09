# Ruby on Rails capstone project - Budget app

## Description

The Ruby on Rails capstone project is about building a mobile web application where you can manage your budget: you have a list of transactions associated with a category, so that you can see how much money you spent and on what. 

You will create an application that allows the user to:
- register and log in, so that the data is private to them.
- introduce new transactions associated with a category.
- see the money spent on each category.

<p align="center">
  <img src="https://github.com/microverseinc/curriculum-rails/raw/main/capstone/images/transactions_list.png" alt="Transactions list page" />
</p>

*IMPORTANT NOTE: Read **all** requirements before you start building your project.*

### General requirements

- Make sure that there are [no linter errors](https://github.com/microverseinc/linters-config).
- Make sure that you used correct [gitflow](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/gitflow.md).
- Make sure that you documented your work [in a professional way](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/documentation/articles/professional_repo_rules.md).

### Programming Language requirements

- Follow the [best practices for the used programming language](link to programming language best practices if available).

### Project requirements

#### Design
- You should follow these [design guidelines](link to the completed figma design by the UI/UX guy), including:
  - Pages.
  - Colors.
  - Typography: font face, size and weight.
  - Layout: composition and space between elements.


The [Creative Commons license of the design](https://creativecommons.org/licenses/by-nc/4.0/) requires that you give appropriate credit to the author. Therefore, you must do it in the README of your project.

#### Interactions
- Splash screen
  - A simple page with the name of your app (yes, you need to choose one), and links to the sign up and log in pages.

- Sign up and log in pages
  - The user should be able to register in the app with full name, email and password (all mandatory).
  - The user can log into the app using email and password.
  - If the user is not logged in, they can't access pages that require the user to be logged in (all the pages described below).

- Home page (catagories page)
  - When the user logs in, they are presented with the categories page.
  - For each category, the user can see their name, icon and the total amount of all the transactions that belongs to that category.
  - When the user clicks (or taps) on a category item, the application navigates to the transactions page for that category.
  - There is a button "add a new category" at the bottom that brings the user to the page to create a new category.

- Transactions page
  - For a given category, the list of transactions is presented, ordered by the most recent.
  - At the top of the page the user could see the total amount for the category (sum of all of the amounts of the transactions in that category).
  - There is a button "add a new transaction" at the bottom that brings the user to the page to create a new transaction.
  - When the user clicks on the "Back" button (<), the user navigates to the home page.

- "Add a new category" page
  - The user fills out a form to create a new category, indicating their name and icon (both mandatory).
  - The user click (or taps) the "Save" button to create the new category, and is taken to the home page on success.
  - When the user clicks on the "Back" button (<), the user navigates to the home page.

- "Add a new transaction" page
  - The user fills out a form to create a new transaction with:
    - name (mandatory)
    - amount (mandatory)
    - categories (mandatory at least one)
  - The user click (or taps) the "Save" button to create the new category, and is taken to the transactions page for that category.
  - When the user clicks on the "Back" button (<), the user navigates to the transactions page for that category.

#### Testing requirements
- Create unit and integration tests for all the most important components of your RoR application.

#### Technical requirements

- You should use Postgres as your database.
- You should use devise for authentication.
- You should validate all user input to make sure that anyone with bad intentions cannot compromise your app.
- You can use a view template engine of your choice (.erb, .slim, .haml).
- The project should be deployed and accessible online.
- Your database schema should reflect the following structure:

> NOTE: do not change column names visible in the diagram. You need to change the "Entity"  name according to the theme you have chosen for your project (please note: "Transaction" is a name already used by ActiveRecord, so using it as a name for your model and table will result in an error).

<p align="center">
  <img src="https://github.com/microverseinc/curriculum-rails/raw/main/capstone/images/erd_diagram.png" alt="ERD diagram" />
</p>

### Project documentation

Once you have finished the development of the project, you should record a video presenting the features of the project you built. It is a video with a **maximum length of 5 minutes**. The content of the video should include:

- a description of the project.
- a demo of the project features.
- you should also highlight some interesting piece of code or something you built that you are very proud of.

For recording the video you can use tools like [Loom](https://www.loom.com/) that let you share a private link to the recording, and configure a shot that shows your computer screen and your face at the same time in a small picture.

## Challenge breakdown

Here is a suggestion of what you can do every day (just a suggestion, not mandatory):

### Day 1
- Set up the repository and tools.
- Create your models according to the ERD diagram. Don't forget about validations and tests.
- Implement the authentication and authorization. 

### Day 2

- Create the page to add a category.
- Create the home page.
- Create the page to add a transaction.
- Create the transactions page.

### Day 3

- Make sure your app is tested adequately.
- Deploy the project, and test for final details.
- Record a video for your project.
- Create a good README and PR description.


## Code review

You will get a code review after each milestone. 

## Additional requirements

- You could implement some UX improvements: include transitions and/or animations, etc.
- Make sure that you have a decent desktop design for the webapp.
- Implement the left side menu to improve the navigability of the app.

------

_If you spot any bugs or issues in this activity, you can [open an issue with your proposed change](https://github.com/wuyepabdul/groove/issues)._
