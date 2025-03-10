# Portfolio

My portfolio is a website to showcase my web development skills, experience and projects. The site is designed to inform potential recruiters and clients about myself and for them to be able to explore my work. It is a digital resume allowing users to be interactive and connect with me about work opportunities.View the live site [here](https://chia-codes.github.io/Portfolio)

MOCK UP IMAGES HERE! ------------------------- 

## Features 

### Site wide
* Navigation Menu
    * Responsive on all devices, the navigation menu will direct you to different pages throughout the site. 
    * This allows users to easily navigate between different pages and sections within the site.  
![Nav Menu](docs/readme_images/navbar.png)

*Header
*  The header is the beginning of my portfolio journey as a user, featuring my name, and a short introduction.
*  The header contains a background image, ensuring engagement for the first impression of the site.
* A call-to-action button is included, allowing user to easily navigate to the ‘send me a message’ page for direct contact.
![Header](docs/readme_images/header.png)

*Footer
* The footer includes icon links to my social media platforms, allowing users to connect across relevant platforms.
* The footer contains contact information, so users can reach out directly.
* The footer includes google maps, display my base location, for users to be informed of my whereabouts.
![Footer](docs/readme_images/footer.png)

* Favicon
    * A customed favicon is used in the browser tap for site branding.
    * This will allow the user to easily identify the site in their browser.
![Favicon](docs/readme_images/favicon.png)

### Landing Page
* Home page
    * Utilising recommended guidelines, the site follows  WCAG 2.1, reassuring accessibility throughout the site.
    * This will contain and about me section where the user can lean and little more about me and my work history. 
    * This will contain a skills section, allowing the user to browse through my relevant skill set and how it relates to me. 
![About](docs/readme_images/about-me.png) 

![Skills](docs/readme_images/skills.png) 


* Contact form
    * This allows users to easily reach out and send me a message. The form will consist of the following fields and attributes: 
        * First Name (required, type=text)
        * Last Name (required, type=text)
        * Email (required, type=email)
        * Radio button options (required)
        * Message (required, type=textarea)
    * Successfully submitting the contact form, users will be redirected to success.html displaying a ‘thank you’ message.
    * A radio button is included for clarity of inquiries, stating weather the user is a client or employer. 
![Message Form](docs/readme_images/send-message.png) 
![Message Form Comfirmation](docs/readme_images/succes.png)

### Portfolio Page
* Portfolio
    * Portfolio page showcases projects worked on with relevant links to site repository and deployment. Clicking on links allows users to see projects in more detail.
    * Each project is displayed on a carousel with captions to inform the user about the imagery.
    * This allows users to browse through past projects and see my obtain knowledge and skills in action.  
![Portfolio](docs/readme_images/portfolio.png) 

### Existing Features

* Responsive content
* Hidden internal page
* External frameworks
* Imported google fonts and map


### Features Left to Implement

* To enhance the use of the site, contact form could be set to directly send message to email with a pop ‘success’ modal.
* Google map to be responsive across all devices.

## Design

### Wireframes
<br>
Home page
<br><br>

HOME PAGE WIREFRAME HERE DESKTOP----------

MOBILE HERE ---

TABLET HERE----
<br><br>
Send message form successful submission page.
<br><br>
MESSAGE WIREFRAME HERE DESKTOP -----------------

MESSAGE WIREFRAME HERE MOBILE -----------------

MESSAGE WIREFRAME HERE TABLET -----------------


Portfolio page
<br><br>
MESSAGE WIREFRAME HERE DESKTOP -----------------

MESSAGE WIREFRAME HERE MOBILE -----------------

MESSAGE WIREFRAME HERE TABLET -----------------


## Technologies
**Languages**
* HTML
    * To build structure and develop the Website.
* CSS3
    * To customise and style site with CSS in an external file.
**Frontend Framwork**
*Bootstrap V5.3
    * To lay foundation and structure to card section and navbar.
**IDE**
* Visual Studio Code
    * The website was created and developed using VS Code.
**Host**
* GitHub
    * Source of the code is hosted on GitHub and deployed using Git Pages.
**External Design**
* Font Awesome
    * Icons obtained from https://fontawesome.com/ used in social media section.
* Favicon.io
    * Favicon files were customised created at https://favicon.io/favicon-converter/ 
**Images**
* Squoosh
    * https://squoosh.com/ was used to reduce the size of the images used throughout the website.
* Balsamiq
    * Website wireframes were created using balsamiq https://balsamiq.com/wireframes/desktop
## Testing
Chrome DevTools was used throughout development and testing the deployed website to check for accessibility issues.

Testing was focused on the following criteria:

- All forms have associated screen-read tags to ensure accessibility of the visually impaired. 
- Heading are not missed or skipped to show importance and meaning of content.
- All images and media content has alternative descriptive text for screen readers.
- Making sure WCAG 2.1 recommended coding practices are being followed.

### Responsiveness

All pages were tested to ensure responsiveness on screen sizes from 320px and upwards on Chrome, Edge, and Firefox.

Steps to test:

1. Open browser and navigate to [Portfolio](https://chia-codes.github.io/portfolio)
2. Open the developer tools (right click and inspect)
3. Set to responsive and decrease to 320px
5. Click and drag the responsive window back and forth to minimum and maximum width.

Expected:

Website is responsive on all sizes and no images are stretched.
No horizontal scroll is present.
No elements overlap.

Actual:

Website behaved as expected with the exception of overlapping unreadable content from navbar dropdown menu and header overlapping ‘About me’ section.

Website was also opened on the following devices and no responsive issues were seen:

- Samsung Galaxy S23
- Amazon Tablet
- iPhone 13
- Dell Desktop-AH44THS

### Accessibility Issues & Fixes
Manual tests were performed to identify problematic issues, they are as follows:

#### Issue #1: Navbar Clear Did Not Close on Click
- **Problem**: The navigation menu remained opening when clicking on skills section and background on items not visable.
- **Fix**: I have not yet found a way to resolve this issue as the code sits the same for all navbar items.

#### Issue #2: Large Images Impacting Loading Time
- **Problem**: Image files where holding excessive data increasing loading time during performance.
- **Fix**: Compressed all image files from ‘png’ to ‘webp’ using squoosh. 

#### Issue #3: Header Image Was Not Present on Mobile
- **Problem**: The header background image was taking too long to load, leading to  poor user experience.
- **Fix**: `preload` in the `<head>` used to load the background image early saving load time.

#### Issue #4: Fonts Loading Slowly
- **Problem**: Imported Google Fonts were slowing down performance.
- **Fix**: Added `<link rel="preconnect"…>` and preloaded critical fonts using `<link rel="preload">` to the head.

#### Issue #5: Unused CSS Cause Slow Performance
- **Problem**: Styles in the CSS file were not being utilised, slowing down load time.
- **Fix**: Used Chrome DevTools – Coverage to manually remove unused CSS

#### Issue #5: Caousel Captions Not Present On Small Devices
- **Problem**: Carousel captions are not visible on small devices.
- **Fix**: This issue is unresolved as it needs to be looked into with bootstrap framework and I am unsure how to do this.
  
![Home](docs/testing/lighthouse-test-home-mobile.png) 

![Send Message](docs/testing/lighthouse-send-message-test.png)

![Portfolio](docs/testing/lighthouse-portfolio-test.png) 


### Functional Testing

**Navigation Links**

Testing performed to make certain all nav links navigate to the correct pages and sections. This was done by clicking on the navigation links on each page.

| Navigation Link | Page to Load    |
| --------------- | --------------- |
| Home            | index.html      |
| About       | about.html |
| Skills         | skills.html    |
| Potrfolio         | portfolio.html    |
| Contact         | send-message.html    |


Links on all pages navigated to the correct pages and section as expected.

**Form Testing**

The form on the home page tested to verify it functioned as expected when correct data was input and when incorrect data was input. 
The following test conducted:

_Scenario One - Correct Inputs_

Steps to test:

1. Navigate to [Portfolio - Home Page](https://chia-codes.github.io/portfolio/index.html)
2. Scroll down to ‘send me a message’ in header’:
3. User will be redirected to [Portfolio – Message Page](https://chia-codes.github.io/portfolio/send-message.html) then input:
   - First Name: Mary
   - Last Name: Anne
   - Email: email@test.com
   - Select any option for radio buttons
   - Comment: This is a test.
3. Click Submit
4. User should be redirected to success.html a confirmation page

Expected:

Form submits with no errors and user is redirected to success.html 

Actual:

No errors present and user is redirected to success.html

_Scenario Two - Missing Any Text Field_

Steps to test:

1. Navigate to [Portfolio - Home Page](https://chia-codes.github.io/portfolio/index.html)
2. Scroll down to ‘send me a message’ in header’:
3. User will be redirected to [Portfolio – Message Page](https://chia-codes.github.io/portfolio/send-message.html) then input:
   - First Name: Mary
   - Last Name: 
   - Email: email@test.com
   - Select any option for radio buttons
   - Comment: This is a test.
3. Click Submit
4. User should be prompted to fill in missing field.


Expected:

The form does not submit and a pop-up is displayed to tell the user that the field is required.

Actual:

Behaved as expected, pop-up message displayed and form did not submit.

_Scenario Three – Radio Buttons Left Empty_

Steps to test:

1. Navigate to [Portfolio - Home Page](https://chia-codes.github.io/portfolio/index.html)

2. Scroll down to ‘send me a message’ in header’:
3. User will be redirected to [Portfolio – Message Page](https://chia-codes.github.io/portfolio/send-message.html) then input:
   - First Name: Mary
   - Last Name: Anne
   - Email: email@test.com
   - Do not select options for radio buttons
   - Comment: This is a test.
3. Click Submit
4. User should be informed radio buttons options are required.


Expected:

The form does not submit and pop-up is displayed to tell the user that an option is required.

Actual:

Site behaved as expected and pop-up message to pick and option is present.

_Scenario Four - Wrong Email Format_

Steps to test:

1. Navigate to [Portfolio - Home Page](https://chia-codes.github.io/portfolio/index.html)

2. Scroll down to ‘send me a message’ in header’:
3. User will be redirected to [Portfolio – Message Page](https://chia-codes.github.io/portfolio/send-message.html) then input:
   - First Name: Mary
   - Last Name: Anne
   - Email: email----test.com
   - Select any option for radio buttons
   - Comment: This is a test.
3. Click Submit
4. User should be informed email is invalid and to input correct format.

Expected:

The form does not submit and a pop-up is displayed to tell the user that the field is not valid.

Actual:

Website behaved as expected, expected pop-up message was displayed and the form did not submit.

**Footer Social Media Icons / Links**

Testing for social media icons was performed to make certain links direct to the correct sites, open in a new tab and has hover effect to reassure the user that it’s a link. 
Each item did opened a new tab when clicked as expected and change in color when hovered was present. All links lead to expected sites. 

**Footer Contact Information**

Testing in the contact section was performed to make certain the user can reach out directly though the site. Phone number to prompt a call action from mobile devices and email to open email application across any device.

_Steps to test Telephone Number_

1. Navigate to [Portfolio - Home Page](https://chia-codes.github.io/portfolio/index.html)
2. Click the contact in navbar or scroll to number in the footer (0208 726 9958)

Expected:

On mobile pop-up should be displayed to call selected number.

Actual:

Behaved exactly as expected and prompted the user to make a phone call with selected number.

_Steps to test Email_

1. Navigate to [Portfolio - Home Page](https://chia-codes.github.io/portfolio/index.html)
2. Click the contact in navbar or scroll to email in the footer (SanchiaN-L@hotmail.co.uk)

Expected:

An email application displays itself with target email address in ‘TO’ section ready to send email. 

Actual:

Behaved as expected and opened a Microsoft application on desktop and outlook app on mobile with target address in ‘send to’ section. 

### Validator Testing 

- HTML
  - 4 Errors found with wrong tag issues as displayed in image below

![Main Page HTML Validator Results](docs/testing/html-validator-error-test.png) 

Fix: Remove unnecessary tags. 

![Main Page HTML Validator Results](docs/testing/html-validator-test.png)

![Potrfolio HTML Validator Results](docs/testing/portfolio-html-validator-test.png)

![Send Message HTML Validator Results](docs/testing/send-message-html-validator-test.png)

![Message Success Results](docs/testing/message-success-html-validator-test.png)

- CSS
  - No errors were found when passing through the official [(Jigsaw) validator]( https://validator.w3.org/)

![CSS Validator Results](docs/testing/css-validator-test.png) 

### Unfixed Bugs
Responsiveness of the website worked on all devices, screen sizes with an exception of unresponsive google map in footer and visual clarity in dropdown menu on navbar items. 

## Deployment

### Version Control

The site was created using the Visual Studio code editor and pushed to github to the remote repository ‘tacos-travels’.

The following git commands were used throughout development to push code to the remote repo:

```git add <file>``` - This command was used to add the file(s) to the staging area before they are committed.

```git commit -m “commit message”``` - This command was used to commit changes to the local repository queue ready for the final step.

```git push``` - This command was used to push all committed code to the remote repository on github.

### Deployment to Github Pages
The portfolio website is deployed using **GitHub Pages** 

### Steps to Deploy:
1. Sync files to a GitHub repository from VS Code.
2. Go to the **Settings** tab in the repository.
3. Scroll down to the **Pages** section.
4. Under **Branch**, select `main`
5. Click **Save**.
The live link can be found here - https://chia-codes.github.io/portfolio

## Credits 

* [Bootstrap](https://getbootstrap.com/)
    * Code was used from this site used to create structural foundtation of navbar and cards custmoised to my relevant preferences and ensure syncrinicity of styling throughout the site.
* [Javascript](https://javascript.com/)  
    * Javascript also deserve ceditation as it was used in conjustion with bootstrap 5.3
* [Squoosh](https://www.squoosh.com)
    * Was used to compress files, coverting them from png to webp increasing site load time.
* [Code Institute](https://learn.codeinstitute.net)
    * Code institute resorces including my mentor (Gareth Mcgirr) help with structural elements and how to code for prefered results.
* [W3 Schools](https://www.w3schools.com)
    * Used to learn, reference and discover code elements to help build site.
* [Slack](https://slack.com/intl/en-gb/)
    * Slack was used to discuss code, fix hosting and connecting issues and gain feedback on written code.
* [Google](https://www.google.com)
    * Used for the site to conatain useful links and fonts. 
      

### Media

* [Pixabay](https://pixabay.com/)
    * Was used to discover royalty free audio embedded in the heade, audio credit goes to Sergei Chetvertnykh from pixabay. 
* [OpenAI](https://www.openai.com)
    * Used to generate personalised and custom imagery throughout the website. 
