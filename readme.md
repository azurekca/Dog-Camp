YelpCamp

Final project for the Web Developer Bootcamp by Colt Steele.

Live project is on Heroku here https://sleepy-everglades-99325.herokuapp.com/


Lessons with video number reference to build each step in this project

1 (291)
  - Add landing page
  - Add ampgrounds page that lists all campgrounds
    Campgrounds have
    - name
    - image

2 Laypout and basic styling (293)
  - Create header and footer partials
  - Add in Bootstrap

3 Creating New Campgrounds (294)
  - Setup new campground post route
  - Add in body-parser
  - Setup route to show form
  - Add basic unstyled form

4 Style the campgrounds page (295)
  - Add a better header/title
  - Make campgrounds display in a grid

5 Style the Navbar and Form (296)
  - Add a navbar to all templates
  - Style the new campground form

6 Add MongoDB/Mongoose (305)
  - Install and configure mongoose
  - Setup campground model
  - Use campground model inside of our routes

7 Show Page (307)
  - Review the RESTful routes we've seen so far
  - Add description to our campground model
  - Show db.collection.drop()
  - Add a show route/template

8 Refactor Mongoose Code (326)
  - Create a models directory
  - Use modules.exports
  - Require everything correctly!!

9 Add the comment model! (330)
  - Make our errors go away
  - Display comments on campground show page

10 Comment New/Create (332)
  - Discuss nested routes
    - nested routes are used when associating data. When we add a comment, it is associated with a campgroud and our route will reflect that.
    - NEW     campgrounds/:id/comments/new    GET
    - CREATE  campgrounds/:id/comments        POST
  - Add the comment new and create routes
  - Add the new comment form

11 Style show page (334)
  - Colt uses Bootstrap 3 and some custom styles
  - I used Bootstrap 4 which didn't require additional custom styles at this point, and I styled it slightly differently

12 Auth Part 1 - Add User Model (344)
  - Install all packages needed for authentication
  - Define User model

13 Auth Part 2 - Register (345)
  - Configure Passport
  - Add register routes
  - Add register template

14 Auth Part 3 - Login (346)
  - Add login routes
  - Add login template

15 Auth Part 4 - Logout/Navbar (347)
  - Add logout route
  - Prevent user from adding a comment if not signed in
  - Add links to navbar

16 Auth Part 5 - Show/Hide Links (348)
  - Show/hide auth links correctly in the navbar

17 Refactor the Routes (349)
  - Use Express router to reorganize all routes
    - here we used a number of new concepts: methods part of express that enable the dividing of routes into separate files, but without having to do the many lines of code requuired to set up express in each file. We did this with express.Router

18 Users + Comments (350)
  - Associate users and comments
  - Save author's name to a comment automatically

19 Users + Campgrounds (351)
  - Prevent an authenticated user from creating a campground
  - Save username and id to newly created campground

20 Editing Campgrounds (353)
  - Add method-override
    - npm package that enables put and delete form requests
  - Add edit route for campgrounds
  - Add link to edit page
  - Add update route

21 Deleting Campgrounds (354)
  - Add destroy route
  - Add delete button

22 Authorization: Campgrounds (356)
  - User can only edit their campgrounds
  - User can only delete their campgrounds
  - Hide/Show edit button

23 Editing Comments (358)
  - Add edit route for comments
  - Add edit button
  - Add update route

24 Deleting Comments (360)
  - Add destroy route
  - Add delete button

25 Authorization: Comments (361)
  - User can only edit their comments
  - User can only delete their comments
  - Hide/Show edit and delete buttons
  - Refactor middleware: we put all the middleware into it's own file

26 Adding in Flash messages
  - Demo of working version
    - This package enables us to show alerts on the page
    - We can use bootstrap (or CSS) to style them nicely
  - Install and configure connect-flash
  - Add bootstrap alerts to header

Additional Features I've Added
  - Fuzzy search: search for campground by name or partial name
  - Time stamps on campgrounds added and comments added, and show page displays how long ago a campground or comment was added
  - Slugs: Semantic URLs for the campgrounds
