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
  - [ y ] Able to add feedback
    - [ y ] Data collected on individual pages & components
    - [ y ] Click on next takes you to the next page in sequence
    - [ y ] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [ y ] Thank you page takes you back to the first view
    - [ y ] Old Data is cleared on form completion

- Client code:
  - [ y ]  Individual components for each form part
  - [ y ]  Redux setup complete
    - [ y ] Store linked to react with `<Provider>`
    - [ y ] Store setup with reducer(s) and logger middleware 
  - [ y ] Reducers & Actions Working
    - [ y ] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [ y ] Actions have a `type` key, and `payload` if sending data
    - [ y ] Reducers are returning a new state, or the old state (not mutating)
    - [ y ] Reducers are using spread correctly (to keep old data, while adding new)
  - [ y ] Review Component shows at all times with current redux state
  - [ y ] React-Redux Working
    - [ y ] Dispatching actions onClick
    - [ y ] Grabbing data from the redux store with `useSelector`
  - [ y ] Axios POST request to add feedback


- Server code:   
  - [ n ] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [ y ] Multiple git commits showing incremental progress
  - [ y ] Commits are descriptive of the changes made or feature added 
  - [ y ] Has .gitignore with node_modules
  - [ y ] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [ y ] Appropriate amount of code comments
  - [ y ] Code is consistently formatted
- Client
  - [ y ] Appropriate use of HTML tags
  - [ y ] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of  _Exceeds Expectations_

- Previous Steps
  - [ y ] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [ y ] user can upate their score for a step
    - [ y ] new score is validated to not be empty
    - [ y ] redux is updated with new score
  - [ y ] user can continue on to review page and submit as in Base Mode


- Admin View
  - [ n ] All entries are visible with correct data from inputs
    - [ n ] Most recent is at the top
  - [ n ] Can Delete an entry
    - [ n ] User is prompted before deleting
  - [ n ] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [ y ] Styling with Material UI
- [ n ] Ability to flag a feedback item on `/admin` for further review
- [ n ] Deployed to Heroku


## Markdown

```
Hey Kong,

General Feedback.
The app works great and is very smooth. Great job on finishing some of the stretch goals. Very well done overall.
---
| Functional Requirements | Complete? |
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | yes |
| Data stored in Redux when navigating from page to page | yes |
| User is notified when trying to leave a blank score | yes |
| Review Component displays scores and comments from current redux state | yes |
| Submit button sends data to the server via Axios | yes |
| Confirmaion Page displays after data is POSTed to the server | yes |
| Button on Confirmation Page clears Redux and starts a new survey | yes |
| Views are broken down into components | yes |

---
### Notes:

Notes on the above Functional Requirements.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | 18 |
| Commits are descriptive of the changes made or feature added | yes |
| Readme file updated | yes |
| Appropriate amount of code comments | yes |
| Code is consistently formatted | yes |
| Server code organized with router & module files | yes |

---
### Notes:

Notes on General Items

```
