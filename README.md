# Prosper I.T. Consulting Internship - Vertigo Theatre Content Management System Web App Code Summary

### 2 week internship through Prosper I.T Consulting

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```
## This project was composed and consisted of the following:

- Theatre Vertigo web app build. They are a portland based theatre company.
- Web app was a CMS (content management system) for easy updates to their database without user needing to have a tech background. 
- 2 week sprint with 5+ other developers.
- Azure Devops for project managment.
- Discord for team communication.
- 10 daily stand up meetings and 2 code retrospectives with other devs and project leader.
- Using Visual Studio with ASP.NET framework, C#, JavaScript, HTML, Razor, CSS with bootstrap, font awesome icons, personal style sheets, and asset stylesheets.
- Database: SQL Server, Code first ADO.NET Entity Framework.

### User Story 1.  *Create text helper method*
- I was tasked with the assignment to create a method that can limit the amount of characters in a word and truncate the end characters with elipsis (...)  (Code snippet below)
- In the future a developer could use this method to limit the amount of characters displayed by passing in a string for display and an integer (integer is amount of charcters allowed to display before word is limited with elipsis).
![TextHelpersMethods1st](https://user-images.githubusercontent.com/92835555/169886887-2c73c2c6-8abd-41db-824d-4930dc5b3f46.png)

### User Story 2.  *Create model* 
- This story I was tasked to create the model class for the rental photo section of the web app, after creating this model I scaffolded the CRUD pages with ADO.NET data entity model mapping and updating the database with the new schema. (Code below)

![ModelLiveProject2](https://user-images.githubusercontent.com/92835555/169889776-ccb315d2-5ebf-45b3-b4ac-8a2837c11905.PNG)

### User Story 3. *CRUD pages update create and edit pages with styling updates*

- For this story I was tasked with updating the create and edit pages with styling updates to match the layout of the entire web app layout.  
- I updated these pages and changed the links into buttons for easy user navigation back to index page or to confirm/submit the form. 
-  I also added a file based input to give user ability to choose a image file to add to their database from their machine. 

Create page after update (below)

![CreateAfterUpdatesLP2](https://user-images.githubusercontent.com/92835555/169926934-e8ef67ed-739c-4203-835b-f04d0f724bfc.PNG)

Edit page after update (below)

![LiveProject2EditpgAfter](https://user-images.githubusercontent.com/92835555/170103249-848adbfe-2015-4eaf-b566-d4bb43ec0fa2.PNG)

### User Story 4. *Photo Image storage and retrieval*

-  I was tasked to give the user ability to store and display the images they upload to their database.
-  For this I updated the controller to take in and store images to the database.  All of these results were then displayed on the index page.  
-  This required storing the image as a byte[] in the database by adding additonal logic to create method.  
-  Within the create method I utilized HttpPostedFileBase class to take in the user file as a parameter from the create form and used the binary reader class to produce a byte[] for storage to database.  
-  For display on the index page using Razor syntax I converted the byte[] into a 64base string combined with the image HTML tag.  
-  Below is Index displaying the results without styling. 
 
![LiveProjectIndexBefore](https://user-images.githubusercontent.com/92835555/169738524-19cdc478-6e8a-4f5c-a6d1-55efb7a4ace6.PNG)

- Controller create method (modified below)
![ControllerCreate](https://user-images.githubusercontent.com/92835555/169740541-c0b89b9c-cb83-4641-85c2-44c5ee4eb435.PNG)

- Byte[] -> 64base string conversion Razor syntax

![64baseStringViewConv](https://user-images.githubusercontent.com/92835555/173281857-fe8dac48-24ec-4271-8fc9-4627d4e49b7b.PNG)


### User Story 5. *CRUD pages Index page styling*
- For this story I was tasked with adding styling to Index page.
- Utilizing bootstrap cards I displayed all the database entities and styled the index page with superior styling and layout.  I also added links within font awesome icons on each card that would lead to 
the delete, update, or edit pages.  These icons only appear on hover. (Index search bar was added in future story.)

![IndexAfter](https://user-images.githubusercontent.com/92835555/169740203-a1481ec7-3940-43bf-b1b1-d2ca82827860.PNG)



### User Story 6.  *CRUD pages Details and Delete styling updates*
- I was tasked with improving the styling on the Delete and Details pages.
- Created multiple color schemes to match project color mock up for unique look.
- Added font awesome icon links to other CRUD pages
- Details page after update (below)
![DetailsLP2](https://user-images.githubusercontent.com/92835555/169930881-0354a5d3-9122-48f7-8b8e-7fdb76a6d60f.PNG)

- Delete page after update (below)
![DeleteLP2](https://user-images.githubusercontent.com/92835555/169931542-80208e75-7005-496c-ac4d-b765171626bd.PNG)

### User Story 7. *Add search bar to index page*
- I was tasked to give the user a search bar on the index page.
- User was given ability to search a rental record by using as a keyword some and/or all of the rental name or rental details.
- All results that don't match the search criteria are hidden from view.
- Additional logic added to index controller method

Additonal controller method logic (below)
![ControllerIndex](https://user-images.githubusercontent.com/92835555/169740532-33a27e75-2064-4d34-9275-0e8f219449d4.PNG)

- Index search display (below)
![IndexSearch](https://user-images.githubusercontent.com/92835555/169740210-3f8471ee-45ab-4528-ac97-d0e45e9d1500.PNG)

### User Story 8. *Text helper word limit method*
- For this story I was tasked in creating a text helper method for further use throughout the app.
-  This method will limit the amount of words printed to console and truncate the sentence with elipsis (...) at the end of the last allowed word in the sentence.
-  In the future a dev could use this method to pass in a string and a integer specifying the amount of words they want to display before the string is limited with elipsis.
- Within the text helper class I added method logic to complete this task. (below)
![TextHelpersMethods2nd](https://user-images.githubusercontent.com/92835555/169887092-5667f8d9-8b6b-46cf-8c32-a17a594b1a2a.png)

### Other updates not included in user stories
- updated edit controller to read and save new image to database
- this gives the user the ability to edit and add new images within the specific record.
- updated edit page with file based input and record image display for retrieval and display. (below)
![ControllerEdit](https://user-images.githubusercontent.com/92835555/169740525-f368d553-6132-4bef-89c9-62e7c9f14e3a.PNG)

![EditUpdateLP2](https://user-images.githubusercontent.com/92835555/169928899-f9d4babf-33c7-496a-ba62-5f13c6a251b9.PNG)

## Overview of Project -
- completed 8 user stories.  
- Safely and accurately followed version control standards.  Daily master branch updates, commiting often and pushing only story requirements, resolved merge conflicts without effecting other team members
- Updated project leader daily with current work, roadblocks, and shared future work plans.
- Followed group naming conventions of CSS variables, classes and branch names for better project organization and cohesiveness.
- Scaffolded and built 5 pages with styling, functionality and CSS layout matching previous website build and themes to create a astectically pleasing UI. 
- Updated controller methods and created multiple helper methods that will be used throughout the entire program. 
- Exponentially increased and solidified ASP.NET MVC concepts.
- - Learned how to work on a project team, compartmentalize tasks to reduce conflicts and build off of eachothers strengths and weaknesses through sharing our journeys daily to improve overall performance. 
