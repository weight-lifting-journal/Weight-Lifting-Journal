# Weight-Lifting-Journal
It's hard to keep track of how many reps you can do for time, or how much you usually deadlift. This app keep it all organized and tracked for you.  



## MVP

- Users can log in and:
  - Can create, 
  - Review,
  - Update, 
  - And delete data on their workouts
- Can create:
  - A name of the exercise amount lifted or reps completed, date, and region of the body exercise targets.


# Before we get started
  1. Create a trello board that has the following columns:
    - Backlog (cool features to add after MVP)
    - To-DO (MVP features go here)
    - Currently Working On: One card at a time should be here
    - HELP: Feeling stuck ? Drop a card and there and I (scrum master) will look over it with you, we're a team after all!
    - All-Done: Huzzah! All done :D
  2. Don't forget to share the trello board with me via email!
    - jlalucescareer123@gmail.com
  3. Please do make your cards specific
    - Adding a checklist inside a specific card to further break down tasks can really help you as you work, and help me!

# Back End: Deploy ASAP
  - Our db will have to hold: ( CRUD Operations will take place on these )
    1. Name of excercise
    2. Reps completed & How many sets as well
    3. Date for each journal
    4. Region of body the workout hits
    - `knex, sqlite3, and express ` are nice for DB handling
  - Also need to include Authentication (this is up to the BE dev: JWT)

# Back-End DB: Workout "Journals"
- The `Journal` will hold a card of `Excercises` (excercise "cards")

__Workout "Journal"__ (CRUD)

  - `id`: number, let DB generate this
  - `Date of Journal`: string of numbers, ( mm/dd/yyyy )
  - `Region of Body`: string, 150 char cap

__Excercise "Card"__ (CRUD)

  - `id`: number, let the DB generate this 
  - `workout id`: number, reference this to the id of the workout journal's id
  - `Name of excercise`: string, cap at 150 chars, __required__
  - `Reps Completed`: number, __required__
  - `Sets Completed`: number, __required__
  
# Back-End DB: Login Auth / Register
- Ability to register / login: use whichever language/framework you prefer here --> some ideas:
  1. `bcrypt.js` & `nodemon`
  2. `express` & `express router`
  3. `jsonwebtoken`
  4. `helmet`


# Front-End: React with/without Redux
- Create a react app that can access the backend endpoints accordingly
- Dependencies: obviously your preference --> some ideas:
  1. `axios`
  2. `react-router-dom`
- If time allows for it, add `react testing`

# Front-End: Logging In
- If user logs in: `re-direct` them to their workouts journal page
- If user registers for the first time: redirect to journal page as well   (if we get to make one, you could redirect them to a `getting started`   page or have a ___modal___ that pops up with a `quick tutorial`)
- Register / Login Form:
  - if done dynamically, the React component will just render a ___slightly___ different form than the normal login page
  - Data persistence so when user logs in / registers, they stay logged in automatically
  - If they are neither logged in they only have accses to the:
    - Home Page & Register Page
    - Display a `Please Log In First page` that gets rendered whenever the user isn't logged in, and is currently on a page that requires login access

# Front-End: Navigation
- Navigation to each function of our website:
  1. Home
  2. Create New Workout Journal
  3. Log Out button
  4. Register Button
- Feel free to add a nice transition animation (the UI designers will definitely have fun with this one, so make their dreams come true!)

# UI: Foundations
- A barebones template would be amazing! Include:
  1. Navigation design
  2. Page layouts
    - Priority for the marketing page (its your assignment :D), login / register forms, navigation
  3. Color scheme
    - Up to you :D as long as it looks great!
  4. Fonts
    - Typography is super important, let your creative mind flow free here

# IOS:
  - I personally do not know anything about the iOS development process
  - I am 95% sure you will be working with the DB and routes built out by our BE developer though so make sure to communicate healthily with said developer!
  - If there is anything any of the team can help you with, do let all of us know!
  - You are a very important role as well, don't count yourself out! 
    - Who has time to go on their computer and do all this mumbo jumbo when they can just do it right from their phone AS they work out

# Steps after Bare-Bones v1.0
- Congrats! We all made it, if you are reading this step, the website / app should function nicely
- If there are `bugs` or `errors` / `warnings` inside our dev tools windows, lets get those sorted out!
  - This also means clearing up all the `console.logs() we have as well lol`
- Its time to add more features!
  - Drop your suggestions in the slack channel we have once we are all done!
  - The first big milestone we would like to cover is the ability to upload the progress pics!
    - Working out doesn't count unless we can see those before/after pictures :D

## Stretch 
- All ears for new ideas once we finish!