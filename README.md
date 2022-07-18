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
  - [ ] Able to add feedback
    - [x] Data collected on individual pages & components
    - [x] Click on next takes you to the next page in sequence
    - [] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [x] Thank you page takes you back to the first view
    - [ ] Old Data is cleared on form completion

- Client code:
  - [x]  Individual components for each form part
  - [x]  Redux setup complete
    - [x] Store linked to react with `<Provider>`
    - [x] Store setup with reducer(s) and logger middleware 
  - [x] Reducers & Actions Working
    - [x] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [x] Actions have a `type` key, and `payload` if sending data
    - [x] Reducers are returning a new state, or the old state (not mutating)
    - [ ] Reducers are using spread correctly (to keep old data, while adding new)
  - [ ] Review Component shows at all times with current redux state
  - [x] React-Redux Working
    - [x] Dispatching actions onClick
    - [x] Grabbing data from the redux store with `useSelector`
  - [Kinda-Functioning] Axios POST request to add feedback


- Server code:   
  - [x] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [12] Multiple git commits showing incremental progress
  - [Could be more specific to what was done] Commits are descriptive of the changes made or feature added 
  - [x] Has .gitignore with node_modules
  - [ ] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [x] Appropriate amount of code comments
  - [x] Code is consistently formatted
- Client
  - [x] Appropriate use of HTML tags
  - [ ] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of  _Exceeds Expectations_

- Previous Steps
  - [x] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [ ] user can upate their score for a step
    - [x] new score is validated to not be empty
    - [ ] redux is updated with new score
  - [ ] user can continue on to review page and submit as in Base Mode


- Admin View
  - [ ] All entries are visible with correct data from inputs
    - [ ] Most recent is at the top
  - [ ] Can Delete an entry
    - [ ] User is prompted before deleting
  - [ ] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [ ] Styling with Material UI
- [ ] Ability to flag a feedback item on `/admin` for further review
- [ ] Deployed to Heroku


## Markdown

```
Hey Nate,

General Feedback.

---
| Functional Requirements | Complete? |
| No | Not posting |
| Multi page form with client side routing and navigation (next button) | YES |
| Data stored in Redux when navigating from page to page | Yes |
| User is notified when trying to leave a blank score | YES |
| Review Component displays scores and comments from current redux state | YES |
| Submit button sends data to the server via Axios | no |
| Confirmaion Page displays after data is POSTed to the server | It would if functioning POST |
| Button on Confirmation Page clears Redux and starts a new survey | YES |
| Views are broken down into components | YES |

---
### Notes:

Notes on the above Functional Requirements.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | no |
| Commits are descriptive of the changes made or feature added | no |
| Readme file updated | no |
| Appropriate amount of code comments | Yes but could also say WHAT the function mentioned is doing. |
| Code is consistently formatted | Yes |
| Server code organized with router & module files | Yes|

---
### Notes:

Notes on General Items

*I liked the layout of your functions and the amount of comments. I wish your comments said the INTENTION of the code was. not just WHAT it was. Would have made it easier to step through. 

* The H tags  in your components are used to convey different levels of emphasis. So I liked that you used both H3 and H4. If using for more than a few lines, consider switching to <p> tags or span if nesting things, and adding emphasis with css font-size, and font-weight

* in feedbackRouter on line 34, you have CAPITAL F in Feedback. when req.body was made lowercase

```
