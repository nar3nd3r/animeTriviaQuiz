# Anime Trivia Quiz 

## Contents 
---
  * [UX (User Experience)](#ux--user-experience-)
    + [Project Goals](#project-goals)
    + [User Goals](#user-goals)
    + [User Stories](#user-stories)
    + [Site Owner Goals](#site-owner-goals)
    + [User Requirements and Expectations](#user-requirements-and-expectations)
    + [Design Choices](#design-choices)
    + [Wireframing](#wireframing)
  * [Technologies Used](#technologies-used)
  * [Features](#features)
  * [Testing](#testing)
  * [Bugs](#bugs)
  * [Deployment](#deployment)
  * [References](#references)
    + [Code References](#code-references)
    + [Investment Information Sources](#investment-information-sources)
    + [Image Sources](#image-sources)
    + [Special Thanks](#special-thanks)

## UX (User Experience) 
---
### Project Goals 
* To build a trivia question web app on anime and manga with multiple choice questions.

### User Goals 
* Have my Japanese anime and manga knowledge challenge.
* Challenge myself to beat my previous high score.
* Have fun!

### User Stories 

* As a **user**, I want the web app to be **easy to use** and **is easy to learn to use**.
* As a **user**, I want to **have fun** without **interruptions from errors or bugs**.
* As a **user**, I want the **questions to be randomised** so I can come back to the **challenge with new questions** every-time. 
* As a **user**, should be able to have my **top score saved** to beat next time or challenge others to do so. 
* As a **user**, I would like to **know my progress** through the test in terms of **how much** of test **has been completed**.

### Site Owner Goals 
* As a **site owner**, to entertain and keep user coming back to take the challenge again to beat the top score.
* As a **site owner**, make the quiz fun for the user!

### User Requirements and Expectations 

**Requirements**
* Web application should be on the header part of front-page to dominate the webpage.
* Should be a one page website that has only web app on display to avoid distracting user from main feature.
* Should be without lag and have good performance to make experience comfortable and easy.
* A start page that displays top score and user presses button to begin quiz.
* End of quiz should show a page to save score by entering name and a choice to restart quiz.

**Expectations**
* Visually appealing website that is easy on the eyes and make the UX very positive emotionally.
* Looks fun and the colour schemes should relax user to enjoy their free time.
* Satisfy all user goals to the best of ability by including all relevant features, user should feel site was very enjoyable.

### Design Choices 
---
**Fonts**

I looked for a simple and asthetically pleasing font to match typical holiday themes of relaxations and good times. I chose [Bubblegum Sans](https://fonts.google.com/specimen/Bubblegum+Sans?preview.text_type=custom&sidebar.open=true&selection.family=Bubblegum+Sans) for all texts and headers. 

**Colours**

I chose to use the [Coolors](https://coolors.co/f72585-b5179e-7209b7-560bad-480ca8-3a0ca3-3f37c9-4361ee-4895ef-4cc9f0) colour scheme generator to find one suitable for this project. Below is a screenshot of the colour scheme. They are colours that are pleasant and to look.

![Colour Scheme](wireframes/animeTriviaQuizColours.png)

**Background Image**

I used a manga panel montage as the background to match the theme of anime/manga in the design of web application.

![manga panel montage](assets/images/animeTriviaBg.jpg)

### Wireframing 

For **wireframing**, I used [Balsamiq](https://balsamiq.com/). I used it to create **simple** wireframes 
showing the basic structure on which I built the website on. Some features maybe removed or added during 
development. 

View wireframes for each device here:

**Start Page**
* [Desktop](wireframes/start-page-desktop.pdf)
* [Tablet](wireframes/start-page-tablet.pdf)
* [Mobile](wireframes/start-page-mobile.pdf)

**Question and Answer Page**
* [Desktop](wireframes/desktop-qa.pdf)
* [Tablet](wireframes/tablet-qa.pdf)
* [Mobile](wireframes/mobile-qa.pdf)

**End Page**
* [Desktop](wireframes/end-page-desktop.pdf)
* [Tablet](wireframes/end-page-tablet.pdf)
* [Mobile](wireframes/end-page-mobile.pdf)

## Technologies Used 
---
**Languages**

* [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
* [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
* [JavaScript](https://en.wikipedia.org/wiki/JavaScript)

**Tools & Libraries**

* [Bootstrap](https://getbootstrap.com/)
* [Google Fonts](https://fonts.google.com/)
* [Gitpod](https://gitpod.io/workspaces/)
* [JQuery](https://jquery.com/) 
* [Popper](https://popper.js.org/)

## Features 
---
**Features** that have been **implemented**:
* Ten questions per quiz attempt
* Multiple choice answers
* Score keeping
* Progress bar

**Features** that will be **implemented** in the **future**:
* Saving and displaying high score at the end of the quiz
* Sound effects 
* Background music 

## Testing 
---

### Game is fun!
**User Story: I want to have fun and enjoy the game.**
* **Plan**<br>Give the user questions that are challenging with varying difficulty levels and ask about a wide variety of anime.
* **Implementation**<br>I have included questions of all difficulty level that are randomly selected in order to catch the user by surprise and challenge them.
* **Test**<br>I asked my sister who is a huge anime and manga fan to test it out. 
* **Results**<br>She found it really fun and challenging. The challenging questions were the most satisfying to solve for her.
* **Verdict**<br>The test has passed all the criteria and works as intended.

### Easy to Learn to Use
**User Story: I want to easily learn how to play the game with little complication.**
* **Plan**<br>Build the quiz game as simple as possible so that no instructions are needed. User learns to use it immediately.
* **Implementation**<br>Kept the UI simple and easy to deal with. Creates an effect on buttons and answer choices to change colour during mouse hover event. This allows users to know what to click. I also avoided including unnecessary features that was not relevant. 
* **Test**<br>I asked my sister to test it out.
* **Results**<br>She immediately was able to start and complete the game without giving her instructions. She said there was no problem.
* **Verdict**<br>The test has passed all the criteria and works as intended.

### Questions are randomly chosen
**User Story: As a user, I want the questions to be randomised so I can come back to the challenge with new questions every-time.**
* **Plan**<br>To selected random question each user begins or proceeds to new question.
* **Implementation**<br>I passed the ```questionData``` variable, containing an array of questions along with their corresponding answers, as argument to ```addQuestion()```. Declared variable ```random``` that selects a random number within the range of the array length. I then used this variable as an index to the ```questionData``` array when selecting each question.
* **Test**<br>I took the quiz 5 times and my sister did it twice.
* **Results**<br>The questions displayed were randomized and rarely appeared.
* **Verdict**<br>The test passed all the criteria and works as intended. It will be more random with addition of more questions in the future.

### Saving and displaying top score to challenge user
**As a user, should be able to have my top score saved to beat next time or challenge others to do so.**
* **Plan**<br>To allow user to save their score and to display high scores to challenge new users or the same user to try it again.
* **Implementation**<br>It has not yet been implemented.
* **Test**<br>I shall test once I have implemented.
* **Results**<br>No results yet.
* **Verdict**<br>It has not been implemented due to lack of time as most of the time was occupied working on the other functionalities. It shall be implemented in the future.


## Bugs 
---
### When answer is clicked, the event is repeated

* **Bug**<br>Each time the user selects an answer, whether it is correct or incorrect, the click event is repeated. The click event repetitions doubled with each additional click the user made. For example, when the user clicks to choose answer to second question, it iterated the click twice and fetches two question instead of just one. On third click, it iterated the click four times and fetched four questions.

* **Fix**<br>I refactored the code so that the fetch request inside the function ```apiQuestion()``` is limited to fetching the data and declaring it in a variable to be passed to ```addQuestion()``` and ```addChoices()``` functions. Before code refactoring, ```apiQuestion()``` also handled the functionality of displaying questions and choices to the quiz. I separated these into their own functions to improve readability so I could find the bug and avoid more potential bugs.<br>As I was writing the code, I used ```console.log()``` with each line of code to see where the bug appeared. It appear where I was using ```addEventListener()``` and for the sake of speed, I used JQuery's click event handler ```.click()``` alongside ```.unbind()``` .

* **Verdict**<br>The click event listener works and the intended result has been achieved. I may return to it in order to improve it further. 

### Slow performance when changing questions

* **Bug**<br>It looks a relatively long time to move on to the next question when the users chose an answer. Within that time period when waiting for the next question, if users clicked on the answer again it would add to the number of questions it was going to retrieve. This in turn added to the time waiting for a new question.

* **Fix**<br>Instead of making a fetch request for each new question, I requested all relevant questions once at the start of application. I declared this data in a variable ```questionData``` and passed it to ```addQuestion()``` function to use it to select a question from the available questions. 

* **Verdict**<br>Performance has enormously improved and the side effect of poor performance, which is the potential for users to click on answer multiple times to increase time delay, has been avoided. 
## Deployment 
---

## References 
---
### Code References 

### Special Thanks 