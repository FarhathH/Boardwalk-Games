# Boardwalk Games
## Objective

This is a project walk through where I combine everything I have learned (HTML, CSS, Bootstrap, custom CSS). Practice for my Milestone Projects and will document everything here like my milestones projects.
<hr>

## Overview
This is a website that shows the user options and information on all sorts of tabletop games.

## Project Planning
Our Business client(s):
* Tabletop games shop and cafe.

Primary business goal:
* Increase in-store foot traffic and customer engagement.

Supporting business goals:
* Showcase the shop services.
* Increase brand awareness.
* Provide essential information. 
* Encourage group visits and event participation.


Who are our users:
* People who love socialising and board games:
  * Students gamers interested in budget-friendly entertainment options and discounts.
  * Families & Casual gamers who are looking for a fun time and relaxed atmosphere.
  * Board game enthusiasts seeking information about game events and new releases.

## Skeleton

Code Institute has already prepared these wireframes for us. This will make it easier to be able to structure the website for all devices.

<p align = "center">
 <img width="526" height="593" alt="wireframes" src="https://github.com/user-attachments/assets/a428aa27-6994-4050-a47f-e78887e3edc4" />
</p>

## Testing

I set up the workspace by creating a repository. I downloaded images, imported google fonts, linked the Bootstrap and Font Awesome kit links.

<p align = "center">
 <img width="1280" height="570" alt="Downloaded google fonts" src="https://github.com/user-attachments/assets/c135ba46-36d4-4bca-9dac-9611692cb0dd" />
 <img width="1280" height="570" alt="linked bootstrap and font awesome kit" src="https://github.com/user-attachments/assets/a01dd123-e242-4938-849f-fefd96d81b83" />
</p>

To check that the all of them functioned properly, I altered the code to perform the following:
* For the Bootstrap links:
  * Copied a piece of code from the documentation website to implement a cross button. The cross button showed up. This confirmed that the Bootstrap links functioned as they should.
* The Google Fonts:
  * I simply assigned the fonts. 'Macondo' for the 'H1' tag and 'Inter' for the 'p' tag. The only thing I needed to look out for was the change in the font-family and making the comparison between the Google Fonts display and the Live Server display. They matched so it is safe to say that the imported link functions.
* Font Awesome Kit link:
  * I copied the 'i-frame' code for the dice into the 'p' tag. All I needed for confirmation was the presence of the D20.
 
<p align ="center">
  <img width="1280" height="570" alt="tested external resources" src="https://github.com/user-attachments/assets/1b6d6dc6-8b1d-4bdf-84e8-04dd69e30ebb" />
</p>

When everything seemed fine, I went onto GitHub to deploy and see the comparison between the Live Server and the deployed seemed like night and day. For the deployed version, what should have had the custom fonts in place, instead had the default font for HTML.
<p align = "center">
 <img width="1280" height="570" alt="Deployment problem" src="https://github.com/user-attachments/assets/73b4e81d-a7a6-43fe-8c94-85bf1bf98fe1" />
</p>

To double check if it was an issue with the imported link or the CSS, I used the CSS file to edit the 'body' tag to have the background colour as turquoise. After updating my repository, I checked the deployed file and nothing happened. I could confirm at that point that there was an error with the file path of the style sheet.
<p align = "center">
  <img width="559" height="284.75" alt="testing to make sure it&#39;s not just the imported link" src="https://github.com/user-attachments/assets/d21b010e-dabe-41c5-9220-8c5d9313624d" />
</p>

Just to be sure there wasn't anything else in the code that was causing any trouble, I put my code through the HTML validator and there didn't seem to be any errors. I chose to inspect the develop tools on my browser afterwards. I scanned through the lines of code and removed the slash at the beginning of the CSS file path. It seemed to have solved the issue.

<p align = "center">
  <img width="319" height="284.75" alt="checked with dev tools" src="https://github.com/user-attachments/assets/311113fd-f080-480e-a964-301df5e4ebf5" />
  <img width="620" height="219" alt="checked on html validator" src="https://github.com/user-attachments/assets/bf1f55dd-0790-41bf-a778-8b33a980c7ee" />
</p>


I decided to test this once again. I decided to alter the CSS file path, reload the deployed website again. The fonts and background colour showed up, but I removed the background colour from the 'body' selector once I knew that it functioned.
<p align = "center">
  <img width="662.5" height="608" alt="commited and checked" src="https://github.com/user-attachments/assets/263f8669-2784-4dfc-97ae-79b28e8dbdd8" />
</p>

Added a navbar and manual tested it. I wanted to check that clicking the links would take me to the correct pages after modifying it. All the links took me to the correct locations. The logo and home nav item took me to the index page and the game link leads to the game library page. I removed the visibility grid made from CSS as it was no longer needed. 

<p align= "center">
 <img width="2560" height="1440" alt="manual-testing-navbar" src="https://github.com/user-attachments/assets/b0ccc1ed-aaaf-4c51-a663-54a1b314d258" />
</p>

I made the booking enquiry page so that the user can finally book a session for themself and their family/friends. Of course, I managed to place the labels and input tags with the correct labels. I knew that to check that the form worked properly. I manually tested the fields, one by one. Everything seemed to be working fine until the error message skipped the events type field.

<p align ="center">
  <img width="756" height="581" alt="testing fields in the form" src="https://github.com/user-attachments/assets/fe899acb-c39a-4b0b-8842-f59d1f67c359" />
</p>

I checked on VS code for the source of the problem. I noticed that the reason for this was that for the events type field code, the default selected keyword was used for the Selected option which caused it to bypass the HTML validation check. By changing the selected keyword to a value with a blank. It was no longer classed as a valid option. After checking again, every field functioned as intended and I was able to submit the right information.

<p align="center">
 <img width="922" height="166" alt="changed the value for selected as a blank so that it isn&#39;t registered as a blank" src="https://github.com/user-attachments/assets/525abcad-a91a-4869-8e88-c9e9a7c0e8ea" />
  <img width="647" height="515" alt="This fixed the issue" src="https://github.com/user-attachments/assets/5efe664c-71cf-42d5-b0c2-315e4b126410" />
</p>

To complete full functionality, I created and added a success.html page that will load for the user after a successful submission. I managed to get this page to load by inserting the link to the page itself in the action attribute. This way the form will go to the page if the submission is successful.

<p align="center">
  <img width="577" height="342" alt="added success html page for successful submission" src="https://github.com/user-attachments/assets/4ee021ae-b683-448f-8bff-a05bb10f70e2" />
</p>

When I implemented the form for the user to reserve a game, I loaded the live server version to check that all of the input fields would activate the html built-in validation check. I was satisfied to see that all the fields functioned as they should and I was able to submit the form as it led me to the success.html page.

<p align="center">
 <img width="1280" height="550" alt="manually tested games selection form" src="https://github.com/user-attachments/assets/3c2a4b80-4f9f-4401-a924-525fecde803a" />
</p>

As soon as I had fulfilled all the user stories criteria, I started manually testing the deployed website and made sure of the following:
All of the nav items in the navbar should take the user to the corresponding pages. 
* The logo takes the user to the homepage.
* All of the booking now buttons take the user to the booking forms.
* Each social-link icon takes the user to the corresponding social media page.
* The website is responsive to all screen sizes.
* All of the forms work.

After testing the deployed website, I noticed that the navbar stayed at the top whenever I scrolled down. The user would have been annoyed that they would have to scroll back up to access the navbar. The events section’s ‘booking now’ button would take me to the enquiry booking form rather than the games reservation booking form. I managed to solve half of the problem by applying the fixed-top class to the nav tag and changing the hyperlink for the ‘book now’ button on the events section.

<p align="center">
 <img width="1104" height="517" alt="made some corrections after manual testing the deployed site" src="https://github.com/user-attachments/assets/ece7db0c-2b95-4749-bb13-ef2e993052fc" />
</p>

Now I needed to get to the top of the page to show again. The best way to achieve this was by using dev tools to check the navbar height and add that to the padding to the top of the body element. After committing the repository, I loaded up the deployed website once again and was relieved to have seen the navbar stick to the top regardless of where the user would scroll. I checked the nav item links. There was one problem. When clicking on the services link, the auto scrolls down to the section, but the title is blocked by the navbar.

<p align="center">
 <img width="947" height="519" alt="checked with dev tools and added 57 55px padding to body" src="https://github.com/user-attachments/assets/456f8389-520d-4bb5-b115-cd56fdb023d8" />
</p>

This was a quick and easy fix. I just replaced the margin properties with the padding-top property to prevent navbar overlap. This did fix the issue. I still continued to manually test all of the functions of the website. There was a new problem. In mobile view, when clicking a service or events nav item the navbar stays expanded and doesn’t minimise. It would be a better user experience if the navbar automatically minimised.

<p align="center">
 <img width="2323" height="806" alt="fixed the overlap issue by replacing margin with padding" src="https://github.com/user-attachments/assets/dafa7b70-9f8a-4ffd-a4d4-a4299937757c" />
</p>

To fix this, I simply applied some JavaScript for the index page only. This ensured that the mobile view, the navbar immediately minimises on the index.html page.

<p align="center">
<img width="742" height="376" alt="Fixed the navbar overlap with javaScript" src="https://github.com/user-attachments/assets/517200b5-29e4-4ce9-99bc-328b0239622b" />
</p>

I double checked and noticed that the buttons for the forms were too close to the footer and the ‘book now’ button on the navbar was the wrong colour. When I looked back in VS code and scanned for the issue. I forgot to add the ‘custom-button filled’ class so I quickly fixed that and added ‘mb-4’ to the submit buttons to add space. It looked less cluttered as a result.

<p align="center">
 <img width="1160" height="722" alt="Fixed manual testing errors" src="https://github.com/user-attachments/assets/f6a37d49-28a2-4180-a532-4b2cbf52eea5" />
</p>

Once I had finished the manual testing for my website. I went ahead to use the lighthouse feature from dev tools to check for any weaknesses and improve my website. I started off with the index.html report. Results were positive, but there were some insights and diagnostics noted in the report. Most of the performance issues were based on the toolkits from Google Fonts and Bootstrap so I couldn’t really do much to fix this. With the accessibility issue, it was mostly down to one of the card images lacking an alt attribute.

<p align="center">
 <img width="790" height="538" alt="lighthouse desktop report" src="https://github.com/user-attachments/assets/bf9d6129-84a0-4b1f-9c8e-682d064f379e" />
</p>

Once I added the missing alt attribute for the card image, I committed the repository and did a hard refresh. I deleted the old  lighthouse report and generated a new one. Accessibility is now at 100. Best practice is at 100 already so I didn’t really need to change and improve anything.

<p align="center">
 <img width="388" height="470" alt="Fixed accessibility through adding the missing alt attribute" src="https://github.com/user-attachments/assets/c19a094a-2903-440d-98e0-4e20b5b16424" />
</p>

I decided to check out the game-library page, the success page and booking form page. Both the booking page and the success page have the highest score for performance, accessibility and best practice. Those two pages were left alone. I decided to scroll through the lighthouse report for the games-library page. The performance score was 84. I looked at the diagnostics and insights. Most of them were the result of using re-built tools on my website like the Bootstrap classes, Google Fonts etc.

<p align="center">
 <img width="835" height="453" alt="lightouse report of other pages" src="https://github.com/user-attachments/assets/2c8e16e3-2f23-43db-a491-ed061e818181" />
</p>

So I moved onto some HTML and CSS validation testing for the website. I started off with the index page and css code. The results showed me that there were no errors with either HTML or the CSS. There was only one typo with the slash in the img tag on line 135. I removed it so it was an easy fix.

<p align="center">
 <img width="1210" height="964" alt="Fixed the issue after getting HTML and CSS validation results for index" src="https://github.com/user-attachments/assets/773f8ba9-92b1-4a9f-ac3d-48dd641ed94c" />
</p>

With the other pages of the website, the only page with some errors was the success page.
Most of the errors noted were the result of a missing closed div tag before the footer closing tag. I remedied that by making the correction.

<p align="center">
 <img width="1263" height="843" alt="Fixed the errors after HTML validation testing" src="https://github.com/user-attachments/assets/a590a55a-2401-479f-8959-0d0bdc731ec2" />
</p>

## Responsive Design
I started off with creating the following sections (though in the earlier stages the navigational bar was not created yet):
* Navigation:
  * Contains logo and navigational items
  * User can access other pages
* Header:
  * Has introductory text and a hero banner.
* Main with sections:
  * Contains info about services
* Footer:
  * Contains location, opening times and contact details.


<p align = "center">
 <img width="360" height="245" alt="laptop screen" src="https://github.com/user-attachments/assets/52b20b24-a76f-4630-92b3-34875922b02a" />
 <img width="401" height="417" alt="tablet and mobile screen" src="https://github.com/user-attachments/assets/e17b1a91-296f-4b60-907a-fe16e7c2a19a" />
</p>

I had created the game-library page by transferring the code from the index page. I did a quick look in the browser developer tools just to see the differences in different screen sizes once again. Everything seemed fine at the moment.

<p align="center">
   <img width="2435" height="820" alt="game-library-page-screen-sizes" src="https://github.com/user-attachments/assets/a6d78146-f4fd-41f9-9ba9-9d303d51fba9" />
</p>

I soon started adding content for the header and a carousel for the index page. I tried to make sure that the heading, subheading and the paragraph are distinct from each other. When I checked in the dev tools, the header content was still responsive to mobile, tablet and laptop screens.
The carousel’s autoscroll worked as well.

<p align="center">
 <img width="2560" height="1440" alt="added-index-header-text-and-tested-responsive-design" src="https://github.com/user-attachments/assets/5a2f5f39-1478-49d9-8ab7-3be46ec6cdbf" />
</p>

I started adding the main section content for the the index and game-library pages.
<p align = "center">
  <img width="208.5" height="304" alt="section services content but the  card height is inconsistent" src="https://github.com/user-attachments/assets/e6bfa164-4e01-496a-b96b-7fa3039becb3" />
  <img width="330.5" height="170" alt="the extra large screen is still inconsistent" src="https://github.com/user-attachments/assets/aff32cf8-e22f-4ad9-93a4-dbb4dbc218b9" />
</p>

<p align="center">
  <img width="208.5" height="304" alt="section services content but the  card height is inconsistent" src="https://github.com/user-attachments/assets/b5c625b5-8b04-4414-8a9b-53ab787a06ad" />
  <img width="406.5" height="269.25" alt="reused the necessary to add content to games-library" src="https://github.com/user-attachments/assets/62780d50-8694-4c66-8089-ab4c7ac9a363" />
  <img width="402.5" height="445" alt="fixed the issue" src="https://github.com/user-attachments/assets/0e905514-7233-4d5a-9a40-40396d942913" />
</p>
Checked the appearance in the mobile/tablet view. Everything seemed to be fine for the most part, but I only had changed the margin for the contact information section to allow breathing room between the contact details and the opening times table. Once that correction was done, I added the footer to the games-library page as well and updated the links in the navbar.
<p align = "center">
  <img width="463" height="854" alt="viewed in mobile view and added top and bottom margin for the contact section" src="https://github.com/user-attachments/assets/d3b1253d-b3df-4757-9f4c-5c74e0f758b1" />
</p>

I finally managed to keep the core features of the homepage. At this point, I thought that adding an events section would be beneficial for the users. I made sure to include rough info about the events that ‘Boardwalk Games’ offers. I made sure to split the paragraphs and table into two columns on larger screen sizes and group them in one column on smaller screen sizes.
<p align="center">
 <img width="960" height="542" alt="Worked on the responsive design of events section" src="https://github.com/user-attachments/assets/49ee8fa7-0352-45a7-9774-1101e7e89d82" />
</p>

After dealing with the events section, I essentially applied the same type of code for the game reserve section form. I did some quick editing of the html and css code to make sure that it was responsive to all screen sizes.
<p align="center">
 <img width="794" height="712" alt="screen sizes of the game reserve section form" src="https://github.com/user-attachments/assets/bd053c2b-ed52-4c8a-b6e5-d180b7d5f0d9" />
</p>

## Accessibility
During the development of getting the navbar for my website sorted, I originally had used a bootstrap template to start off by changing the style by using some custom CSS and removing the 'bg-body-tertiary' class that was put by default as it was overriding it.

<p align="center">
 <img width="653" height="213" alt="changed-navbar-colour" src="https://github.com/user-attachments/assets/5a57c61e-8b14-40d4-bd97-d756e13fe62d" />
<img width="702" height="39" alt="changed-font-color-for-good-contrast" src="https://github.com/user-attachments/assets/1708ad49-c452-4f64-adbb-b0f7b08d209b" />
</p>

Added contact info in the footer and added background colour. At this stage, I just wanted to get the rough info in place. The only problem was that the font for the address and contact details was too dark and didn’t have enough contrast and that made it difficult for users to read the information.
<p align="center">
  <img width="670" height="184" alt="Added contact info in footer and added background colour with css" src="https://github.com/user-attachments/assets/3de47442-43ba-42ee-a6e0-88230d142f35" />
</p>
So I changed the colour to white for better contrast and applied it to the icons as well. But the main header was invisible. Earlier, I set the font colour for the main heading to be brown. It was hidden in the background as a result. 
<p align="center">
  <img width="566.5" height="183.5" alt="changed the color property for better contrast" src="https://github.com/user-attachments/assets/e9bd419b-0b9e-4bad-9190-f5ecb1dc31cc" />
</p>
So I changed the h2 header colour to white. The same colour as the address and contact information. The user could finally see the title which was notified that the contact information is located here.
<p align="center">
 <img width="495.5" height="203.5" alt="changed h2 heading to white" src="https://github.com/user-attachments/assets/6734b8cb-4c53-4c9e-9422-185248bde1ef" />
</p>
The blue social network icons were small and had lines between them.The colour wasn’t complementary with the background so I added brown to my social network icons for the footer and made them a lighter shade for better contrast.
<p align="center">
 <img width="382" height="183" alt="added light brown shade to my social icons" src="https://github.com/user-attachments/assets/a77f7c4e-38fc-4db1-ba3a-b1735841bf72" />
</p>
I didn’t quite like the look of the light brown icons so I edited it so that the icons for the contact info are white and the social network icon links are light blue. This worked to distinguish between the icons to represent the contact details and the social links that open to the companies’ social homepages.
 <p align = "center">
 <img width="481" height="198" alt="edited so that the icons are light brown and the social links are a light blue" src="https://github.com/user-attachments/assets/4283a7e9-8f10-4739-b5f9-6d05281fbd48" />
 </p>

 For the form, I decided to custom style the buttons. The default blue colour used before didn’t match the colour scheme. So I used the same colour as the subheading font. I also applied the hover effect for the user to know that they can click on it to go to the booking page.

 <p align="center">
   <img width="584" height="373" alt="styled buttons" src="https://github.com/user-attachments/assets/a47e5ef3-4f6a-4533-bd67-069c69a456ba" />
 </p>







