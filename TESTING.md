# The Office Workers Guide To: Cardiff - Testing
![Image](resources/mockups.png)

---
## Contents
- [The Office Workers Guide To: Cardiff - Testing](#the-office-workers-guide-to-cardiff---testing)
  - [Contents](#contents)
  - [Responsiveness](#responsiveness)
    - [Mobile Screenshots](#mobile-screenshots)
    - [Tablet Screenshots](#tablet-screenshots)
    - [Desktop Screenshots](#desktop-screenshots)
    - [Summary](#summary)
  - [Automated Testing](#automated-testing)
    - [W3C Validator](#w3c-validator)
    - [Lighthouse](#lighthouse)
  - [Browser Compatibility](#browser-compatibility)
  - [Manual Testing](#manual-testing)
    - [Testing User Stories](#testing-user-stories)
      - [New User](#new-user)
      - [Returning User](#returning-user)
    - [Full Testing](#full-testing)
      - [Internal](#internal)
      - [External](#external)
  - [| The Gym Group Link |](#-the-gym-group-link-)
  - [Bugs](#bugs)
    - [Solved Bugs](#solved-bugs)
    - [Known Bugs](#known-bugs)
---
## Responsiveness
### Mobile Screenshots
![Image](/resources/testing/mobile-responsive.png)
### Tablet Screenshots
![Image](/resources/testing/tablet-responsive.png)
### Desktop Screenshots
![Image](/resources/testing/desktop-responsive.png)
### Summary
![Image](/resources/testing/responsive-summary.png)

---
## Automated Testing
### W3C Validator
---
### Lighthouse
---
## Browser Compatibility
---
## Manual Testing
### Testing User Stories
#### New User
| Goals | How they are achieved |
| :-----| :--------------------:|
| I want a website that is clear and well organized. |  |
| I want all aspects of the website to be fully functional. |  |
| I want to find out which mode of transport is suitable for me. |  |
| I want to find out what the city looks like. |  |
| I want to be able to find information about other facilities in the city. |  |
| I would like to advertise on the website. |  |
#### Returning User
| Goals | How they are achieved |
| :---- | :--------------------:|
| I want to be able to find alternative modes of transport should my usual mode not be available. | |
| I want to find new places to take lunch. |  |
| I would like the information supplied to be accurate with an option to feedback any incorrect information. |  |
| I would like to be able to quickly navigate through the website. |  |
### Full Testing
#### Internal
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| :-----: | :--------------: | :---------------: | :----: | :-------: |
| **_Navbar_** |
| Logo | When clicked the user will be redirected to the home page.|Clicked Logo on all pages. | Redirected to the home page. | Pass |
| Home Link | When clicked the user will be redirected to the home page. | Clicked link on all pages. | Redirected to the home page. | Pass |
| Commute Link |
| Lunch Link |
| Fitness Link |
| Gallery Link|
| Feedback Link|
|**_Footer_** | 
| Home Link |
| Commute Link |
| Lunch Link |
| Fitness Link |
| Gallery Link |
| Feedback Link |
|**_Home_**| 
| Commute Link |
| Travel Link |
| Lunch Link |
| Gallery Link |
| Feedback Link |
|**_Feedback_** |
| Submit Button |
|**_Thank You_** |
| Home page redirection. |

#### External
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| :-----: | :--------------: | :---------------: | :----: | :-------: |
|**_Home_** |
| YouTube Video |
|**_Commute_** |
| TFW Website x3 |
| Embedded Google Maps|
| Google Maps Link |
| Cardiff Council Link |
| Cardiff Bus Link |
| OVO Bikes Link |
|**_Lunch_** |
| Pasture Link |
| Grazing Shed Link |
| Las Iguanas Link |
| Cosy Club Link |
| Bombers Link |
| 200 Degrees Link |
| New York Deli Link |
| Uncommon Ground Link |
|**_Fitness_** |
| PureGym Link |
| The Gym Group Link |
---
## Bugs
### Solved Bugs
| Bug | Solution |
|:----| :------: |
|Colors not changing from Bootstrap default colors with class attribute| Change the Color at the property value root level in CSS. |
|Initially, the footer was positioned at the bottom of the thank you page using the position: fixed property with left: 0 and bottom: 0. However, during mobile testing, it was observed that the footer overlapped the thank you text, causing visibility issues. | To address the issue of the footer overlapping content on mobile devices, the Bootstrap documentation provided a solution using the flex classes. |
|The placeholder text assigned to a textarea element is not being displayed within the textarea box.| Due to Prettier formatting, the newline character between the opening and closing tags causes the placeholder text to be affected, resulting in an undesired line break.To resolve this issue, the textarea and all of its attributes are placed on the same line in the code.

### Known Bugs


