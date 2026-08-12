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

## Accessibility
During the development of getting the navbar for my website sorted, I originally had used a bootstrap template to start off by changing the style by using some custom CSS and removing the 'bg-body-tertiary' class that was put by default as it was overriding it.

<p align="center">
 <img width="653" height="213" alt="changed-navbar-colour" src="https://github.com/user-attachments/assets/5a57c61e-8b14-40d4-bd97-d756e13fe62d" />
<img width="702" height="39" alt="changed-font-color-for-good-contrast" src="https://github.com/user-attachments/assets/1708ad49-c452-4f64-adbb-b0f7b08d209b" />
</p>

Added contact info in footer and added background colour.
<p align="center">
  <img width="1340" height="368" alt="Added contact info in footer and added background colour with css" src="https://github.com/user-attachments/assets/3de47442-43ba-42ee-a6e0-88230d142f35" />
</p>

Changed the colour for better contrast. But the main header was invisible.
<p align="center">
  <img width="1133" height="367" alt="changed the color property for better contrast" src="https://github.com/user-attachments/assets/e9bd419b-0b9e-4bad-9190-f5ecb1dc31cc" />
</p>

So I changed the h2 header colour to white.
<p align="center">
 <img width="991" height="407" alt="changed h2 heading to white" src="https://github.com/user-attachments/assets/6734b8cb-4c53-4c9e-9422-185248bde1ef" />
</p>

Added brown to my social icons for the footer and made them a lighter brown for better contrast.
<p align="center">
 <img width="764" height="366" alt="added light brown shade to my social icons" src="https://github.com/user-attachments/assets/a77f7c4e-38fc-4db1-ba3a-b1735841bf72" />
</p>

 Edited it so that the icons for the contact info are light brown and the social icon links are a light blue.
 <p align = "center">
 <img width="962" height="396" alt="edited so that the icons are light brown and the social links are a light blue" src="https://github.com/user-attachments/assets/4283a7e9-8f10-4739-b5f9-6d05281fbd48" />
 </p>






