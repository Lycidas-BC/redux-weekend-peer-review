# Weekend Challenge 11 - React-Redux Feedback Form

## Instructions

Reviewing code is an important role developers play. We're going to practice reviewing code from others.

- Get the repo url from your partner
- Get your partner's project running on your computer
- Review the code from your partner and give relevant feedback
- Complete the Markdown section and submit that in the notes section on the assignment app. (Make sure you include who's code you reviewed.)

Practicing compassionate code reviews is important (you can learn more from this video on the topic: https://www.youtube.com/watch?v=Ea8EiIPZvh0 )

## Review Checklist

## Base Required Features 

- Multi-Part Form:  
  - [X] Able to add feedback
    - [X] Data collected on individual pages & components
    - [X] Click on next takes you to the next page in sequence
    - [X] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [X] Thank you page takes you back to the first view
    - [X] Old Data is cleared on form completion

- Client code:
  - [X]  Individual components for each form part
  - [X]  Redux setup complete
    - [X] Store linked to react with `<Provider>`
    - [X] Store setup with reducer(s) and logger middleware 
  - [X] Reducers & Actions Working
    - [X] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [X] Actions have a `type` key, and `payload` if sending data
    - [X] Reducers are returning a new state, or the old state (not mutating)
    - [ ] Reducers are using spread correctly (to keep old data, while adding new)
  - [X] Review Component shows at all times with current redux state
  - [X] React-Redux Working
    - [X] Dispatching actions onClick
    - [X] Grabbing data from the redux store with `useSelector`
  - [X] Axios POST request to add feedback


- Server code:   
  - [X] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [X] Multiple git commits showing incremental progress
  - [X] Commits are descriptive of the changes made or feature added 
  - [X] Has .gitignore with node_modules
  - [ ] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [X] Appropriate amount of code comments
  - [X] Code is consistently formatted
- Client
  - [X] Appropriate use of HTML tags
  - [X] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of  _Exceeds Expectations_

- Previous Steps
  - [X] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [X] user can update their score for a step
    - [X] new score is validated to not be empty
    - [X] redux is updated with new score
  - [X] user can continue on to review page and submit as in Base Mode


- Admin View
  - [ ] All entries are visible with correct data from inputs
    - [ ] Most recent is at the top
  - [ ] Can Delete an entry
    - [ ] User is prompted before deleting
  - [ ] Axios GET request to get all feedback for `/admin` view in componentDidMount
  - [X] Tim showed me some of this functionality in a branch, but has not pushed it to main

  Busywork Goals, consider removing or making more useful

- [X] Styling with Material UI
- [ ] Ability to flag a feedback item on `/admin` for further review
- [ ] Deployed to Heroku


## Markdown

```
Hey __YOUR_TIM_HERE__,

Looks really good! I love that you took the time to think about mobile functionality. Your material-ui radio, edit, and submit buttons look great.

---
| Functional Requirements | Complete? |
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | yes |
| Data stored in Redux when navigating from page to page | yes |
| User is notified when trying to leave a blank score | yes |
| Review Component displays scores and comments from current redux state | yes |
| Submit button sends data to the server via Axios | yes |
| Confirmation Page displays after data is POSTed to the server | yes |
| Button on Confirmation Page clears Redux and starts a new survey | yes |
| Views are broken down into components | yes |

---
### Notes:

Your router has a typo in its console.log on line 9 ("req.boy" instead of "req.body"), hence that undefined we were seeing. Other than that, great logs, comments, and organization. You have a clean and readable style of coding. Your comments are concise and descriptive.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | yes |
| Commits are descriptive of the changes made or feature added | yes |
| Readme file updated | no |
| Appropriate amount of code comments | yes |
| Code is consistently formatted | yes |
| Server code organized with router & module files | yes |

---
### Notes:

You commit regularly and your commit messages are concise and descriptive. Also, way to use branches for stretch goals!

```
