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
