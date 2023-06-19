# The Office Workers Guide To: Cardiff - Testing
![Image](resources/mockups.png)

---
**Contents**
- [The Office Workers Guide To: Cardiff - Testing](#the-office-workers-guide-to-cardiff---testing)
  - [Responsiveness](#responsiveness)
    - [Mobile Screenshots](#mobile-screenshots)
    - [Tablet Screenshots](#tablet-screenshots)
    - [Desktop Screenshots](#desktop-screenshots)
    - [Summary](#summary)
  - [Automated Testing](#automated-testing)
    - [W3C Validator](#w3c-validator)
    - [Validation Summary](#validation-summary)
    - [Lighthouse](#lighthouse)
    - [Wave](#wave)
  - [Browser Compatibility](#browser-compatibility)
  - [Manual Testing](#manual-testing)
    - [Testing User Stories](#testing-user-stories)
      - [New User](#new-user)
      - [Returning User](#returning-user)
    - [Full Testing](#full-testing)
      - [Internal Interactive Elements](#internal-interactive-elements)
      - [3rd Party Links](#3rd-party-links)
  - [Bugs](#bugs)
    - [Solved Bugs](#solved-bugs)
    - [Known Bugs](#known-bugs)
---
## Responsiveness
This website has been tested on a wide variety of screen sizes across multiple manufacturers due to the variations between them. It is important to test the responsiveness of the website due to the  increasing use of mobile devices.  A responsive website ensures a consistent  user experience across different screen sizes and resolutions, allowing visitors to access and navigate the site easily and provides a user-friendly experience regardless of the device being used. Also a responsive design improves search engine optimization (SEO), as search engines prioritize mobile-friendly sites in their rankings.

The resolutions tested as as follows:\
Galaxy S III: 360 x 640\
Iphone SE: 375 x 667\
Iphone 12 Pro: 390 x 844\
Moto G Power: 412 x 823\
Ipad: 768 x 1024\
Nexus 10: 800 x 1280\
Desktop 1080p: 1920 x 1080

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
Testing has been completed using the W3C code validators to ensure that the code used is clean, consistent and  adheres to best practices. No warnings or error were found and the results are shown below.

[Home Page Validation](/resources/testing/validations/index-validation.png)\
[Commute Page Validation](/resources/testing/validations/commute-validation.png)\
[Lunch Page Validation](/resources/testing/validations/lunch-validation.png)\
[Fitness Page Validation](/resources/testing/validations/fittness-validation.png)\
[Gallery Page Validation](/resources/testing/validations/gallery-validation.png)\
[Feedback Page Validation](/resources/testing/validations/feedback-validation.png)\
[Thank You Page Validation](/resources/testing/validations/thank-you-validation.png)\
[404 Page Validation](/resources/testing/validations/error-validation.png)\
[CSS Validation](/resources/testing/validations/css-validation.png)
### Validation Summary
![Image](/resources/testing/validations/validations.png)

---
### Lighthouse
![Image](resources/testing/lighthouse-tests.png)
| Page | Observations |
|:---------- | :--------------- |
| Home Page | In order to address performance issues related to the embedded YouTube video and improve lighthouse testing results, it is recommended to consider using facades. Additional information can be found in the Google documentation, specifically in the section on third-party facades (https://developer.chrome.com/en/docs/lighthouse/performance/third-party-facades/). However, despite attempting to implement the recommended solution, I encountered difficulties in getting the video to render correctly. As a result, I have decided to stick with the original embedded code, which renders correctly and remains responsive.  |
| Gallery Page | During the initial testing of the gallery page, a performance score of 74 was obtained. Upon analysing the results, it became evident that the issue was with the large size of the images used. To address this, I obtained smaller versions of the same images and applied compression to reduce their file sizes. Upon retesting the page, the performance score significantly improved to 99. ![Image](resources/testing/lighthouse-gallery-updated.png)|

---
### Wave
The Wave Tool has been used throughout this project. It has helped us identify and address potential accessibility issues throughout the development process. 

Currently, the Wave Tool has detected an error on the thank you page. This error is a result of the automatic redirection to the home page. While the redirection feature provides a valuable user experience, it triggers an issue with the Wave Tool's evaluation.

The automatic redirection function adds significant value to our users, by automatically redirecting them to the home page without requiring any additional input. This will enhance the overall convenience and efficiency of their browsing experience.

---
## Browser Compatibility
Testing has been carried out on the browsers within the below table as these browsers are most used but in addition to this Firefox uses Gecko rendering engine while the others use WebKit.

![Image](resources/testing/browser-testing.png)

---
## Manual Testing
### Testing User Stories
#### New User
| Goals | How they are achieved |
| :-----| :--------------------:|
| I want a website that is clear and well organized. | This website contains a collection of information topics, each with its dedicated page. Each page is organized into subsections, facilitating easy navigation and making it effortless to find the desired information. |
| I want all aspects of the website to be fully functional. | The interactive elements of the website have undergone thorough testing and have successfully passed all tests. Additionally, the responsiveness of the website has been extensively tested, ensuring it is fully responsive across various devices.  |
| I want to find out which mode of transport is suitable for me. | To access commuting information, users can simply click on the provided link within the commuting section of the home page or the commute link in the navbar. This will redirect them to the dedicated commute page, where all available options are displayed. Users can conveniently gather additional information about their desired options by clicking on the relevant links provided. |
| I want to find out what the city looks like. | To access the gallery, users can simply click on the provided link within the gallery section of the home page or the gallery link in the navbar. This will redirect them to the dedicated gallery page, where all photographs are displayed.  |
| I want to be able to find information about other facilities in the city. | This website provides comprehensive information about various facilities, including lunches and fitness options. Users can conveniently access this information either from the home page or by clicking on the corresponding links in the navbar. Upon clicking a specific link, users will be redirected to the corresponding page, where they can explore further options within their area of interest. |
| I would like to advertise on the website. | To advertise, users can access the feedback section located at the bottom of the homepage or simply click on the feedback link in the navbar. By filling out and submitting the provided form, users can share their information for advertising purposes. |
#### Returning User
| Goals | How they are achieved |
| :---- | :--------------------:|
| I want to be able to find alternative modes of transport should my usual mode not be available. | To explore alternative commuting options, users can click on the link provided in the commuting section of the home page or the commute link in the navbar. This action will redirect them to the dedicated commute page, where all available options are displayed. Users can then browse through the alternatives and conveniently access further information by visiting the respective websites. |
| I want to find new places to take lunch. | Users have multiple ways to access information about dining options. They can navigate to the lunch section on the home page and click on the corresponding link to be redirected to the dedicated lunch page. Alternatively, users can directly use the lunch link provided in the navbar to access the lunch page. On the lunch page, they will find a wide range of places to eat, and by clicking on the links of various restaurants, users can gather detailed information and even make bookings. |
| I would like the information supplied to be accurate with an option to feedback any incorrect information. | It is possible that some information may not always be completely up-to-date. In such cases, we encourage users to navigate to the feedback section and fill out the form to notify us about any incorrect information they come across.  |
| I would like to be able to quickly navigate through the website. | Users have various options to navigate through the website. They can explore the different sections available on the home page to find the desired information. Alternatively, if users already know where the required information is located, they can efficiently utilize the navbar and footer to quickly navigate to the specific page they need. |
### Full Testing
#### Internal Interactive Elements
**Navbar**
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| :-----: | :--------------: | :---------------: | :----: | :-------: |
| Logo | When clicked the user will be redirected to the home page.|Clicked Logo on all pages. | Redirected to the home page. | Pass |
| Home Link | When clicked the user will be redirected to the home page. | Clicked link on all pages. | Redirected to the home page. | Pass |
| Commute Link | When clicked the user will be redirected to the commute page. | Clicked link on all pages. | Redirected to the commute page. | Pass |
| Lunch Link | When clicked the user will be redirected to the lunch page. | Clicked link on all pages. | Redirected to the lunch page. | Pass |
| Fitness Link | When clicked the user will be redirected to the fitness page. | Clicked link on all pages. | Redirected to the fitness page. | Pass |
| Gallery Link| When clicked the user will be redirected to the gallery page. | Clicked link on all pages. | Redirected to the gallery page. | Pass |
| Feedback Link| When clicked the user will be redirected to the feedback page. | Clicked link on all pages. | Redirected to the feedback page. | Pass |

**Footer** 
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| :-----: | :--------------: | :---------------: | :----: | :-------: | 
| Home Link | When clicked the user will be redirected to the home page. | Clicked link on all pages. | Redirected to the feedback page. | Pass |
| Commute Link | When clicked the user will be redirected to the commute page. | Clicked link on all pages. | Redirected to the commute page. | Pass |
| Lunch Link | When clicked the user will be redirected to the lunch page. | Clicked link on all pages. | Redirected to the lunch page. | Pass |
| Fitness Link | When clicked the user will be redirected to the fitness page. | Clicked link on all pages. | Redirected to the fitness page. | Pass |
| Gallery Link | When clicked the user will be redirected to the gallery page. | Clicked link on all pages. | Redirected to the gallery page. | Pass |
| Feedback Link | When clicked the user will be redirected to the feedback page. | Clicked link on all pages. | Redirected to the feedback page. | Pass |

**Home Page** 
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| :-----: | :--------------: | :---------------: | :----: | :-------: |
| Commute Link |  When clicked the user will be redirected to the commute page. | Clicked link on home page. | Redirected to the commute page. | Pass |
| Lunch Link | When clicked the user will be redirected to the lunch page. | Clicked link on home page. | Redirected to the  lunch page. | Pass |
| Fitness Link | When clicked the user will be redirected to the fitness page. | Clicked link on home page. | Redirected to the fitness page. | Pass |
| Gallery Link | When clicked the user will be redirected to the gallery page. | Clicked link on home page. | Redirected to the gallery page. | Pass |
| Feedback Link | When clicked the user will be redirected to the feedback page. | Clicked link on home page. | Redirected to the feedback page. | Pass |

**Commute Page**
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| :-----: | :--------------: | :---------------: | :----: | :-------: |
| Accordion | When clicked the accordion will open and collapse. | Clicked all accordion arrows.| Accordion opened and collapsed as required. | Pass |

**Feedback Page** 
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| :-----: | :--------------: | :---------------: | :----: | :-------: |
| Submit Button |  When clicked the user will be redirected to the thank you page. | Clicked the submit button. | Redirected to the thank you page. | Pass |

**Thank You Page** 
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| :-----: | :--------------: | :---------------: | :----: | :-------: |
| Home page redirection. |  When the thank you page is displayed the user will automatically be redirected to the home page after 30 seconds. | Displayed thank you page. | Redirected to home page after 30 seconds. | Pass |

#### 3rd Party Links
**Home Page**
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| :-----: | :--------------: | :---------------: | :----: | :-------: |
| YouTube Video | When clicked the video will start to play. | Clicked the YouTube play button. | Video started playing. | Pass |

**Commute Page** 
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| :-----: | :--------------: | :---------------: | :----: | :-------: |
| TFW Website x3 | When clicked the user will be redirected to the TFW website in a new tab. |  Clicked the TFW link. | TFW website opens in a new tab. | Pass |
| Embedded Google Maps| The user is able to interact with the map using the zoom controls and by clicking on the map. | Clicked zoom controls and and various locations on the map. | Map zoomed in and out, clicked locations showed further information. | Pass | 
| Google Maps Link | When clicked the user will be redirected to the google maps website in a new tab. | Clicked the google maps link. | google maps website opens in a new tab. | Pass |
| Cardiff Council Link | When clicked the user will be redirected to the Cardiff council website in a new tab. | Clicked the Cardiff council link. | Cardiff council website opens in a new tab. | Pass |
| Cardiff Bus Link | When clicked the user will be redirected to the Cardiff bus website in a new tab. | Clicked the Cardiff bus link. | Cardiff bus website opens in a new tab. | Pass |
| OVO Bikes Link | When clicked the user will be redirected to the OVO Bikes website in a new tab. | Clicked the OVO Bikes link. | OVO Bikes website opens in a new tab. | Pass |

**Lunch Page** 
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| :-----: | :--------------: | :---------------: | :----: | :-------: |
| Pasture Link | When clicked the user will be redirected to the Pasture website in a new tab. | Clicked the Pasture link. |Pasture website opens in a new tab. | Pass |
| Grazing Shed Link | When clicked the user will be redirected to the Grazing Shed website in a new tab. | Clicked the Grazing Shed link. | The Grazing Shed website opens in a new tab. | Pass |
| Las Iguanas Link | When clicked the user will be redirected to the Las Iguanas website in a new tab. | Clicked the Las Iguanas link. | Las Iguanas website opens in a new tab. | Pass |
| Cosy Club Link | When clicked the user will be redirected to the Cosy Club website in a new tab. | Clicked the Cozy Club link. | Cozy Club website opens in a new tab. | Pass |
| Bombers Link | When clicked the user will be redirected to the Bombers website in a new tab. | Clicked the Bombers link. | Bombers website opens in a new tab. | Pass |
| 200 Degrees Link | When clicked the user will be redirected to the 200 Degrees website in a new tab. | Clicked the 200 Degrees link. | 200 Degrees website opens in a new tab. | Pass |
| New York Deli Link | When clicked the user will be redirected to the New York Deli website in a new tab. | Clicked the New York Deli link. | New York Deli website opens in a new tab. | Pass |
| Uncommon Ground Link | When clicked the user will be redirected to the Uncommon Ground website in a new tab. | Clicked the Uncommon Ground link. | Uncommon Ground website opens in a new tab. | Pass |

**Fitness Page** 
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| :-----: | :--------------: | :---------------: | :----: | :-------: |
| PureGym Link | When clicked the user will be redirected to the PureGym website in a new tab. | Clicked the PureGym link. | PureGym website opens in a new tab. | Pass |
| The Gym Group Link | When clicked the user will be redirected to the Gym Group website in a new tab. | Clicked the Gym Group link. | The Gym Group website opens in a new tab. | Pass |

---
## Bugs
### Solved Bugs
| Bug | Solution |
|:----| :------: |
|Colors not changing from Bootstrap default colors with class attribute| Change the Color at the property value root level in CSS. |
|Initially, the footer was positioned at the bottom of the thank you page using the position: fixed property with left: 0 and bottom: 0. However, during mobile testing, it was observed that the footer overlapped the thank you text, causing visibility issues. | To address the issue of the footer overlapping content on mobile devices, the Bootstrap documentation provided a solution using the flex classes. |
|The placeholder text assigned to a textarea element is not being displayed within the textarea box.| Due to Prettier formatting, the newline character between the opening and closing tags causes the placeholder text to be affected, resulting in an undesired line break.To resolve this issue, the textarea and all of its attributes are placed on the same line in the code.
|Through testing  a display inconsistency within the "featured item" section on the lunch.html page has been found, specifically when viewed in the Safari browser. The height of this section appears different in Safari compared to other browsers. | A h-100 class has been added to the featured item section in order for it to render the same across all browsers. 

### Known Bugs
* None 


