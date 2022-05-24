# VertigoTheatreCMS_CodeSummary

## This project was consisted and composed of the following:

- Theatre Vertigo web app build. They are a portland based theatre company.
- Web app was a CMS (content management system) for easy updates to their database without need to have a tech background.  
- 2 week sprint with 5 other developers
- Using Visual Studio with ASP.NET framework, C#, HTML , CSS with bootstrap and font awesome icons, personal style sheets and javascript.
- Database: SQL server Code first ADO.NET entity data model.
- Utilized Azure DevOps for project structure and git for source control.

### User Story 1.  *Create text helper method*
- I was tasked with the assignment to create a method that can limit the amount of characters in a word and truncate the end characters with elipsis (...) (Code snippet below)
![TextHelpersMethods1st](https://user-images.githubusercontent.com/92835555/169886887-2c73c2c6-8abd-41db-824d-4930dc5b3f46.png)
### User Story 2.  *Create model* 
- This story I was tasked to create the model class for the rental photo section of the web app, after creating this model I scaffolded the CRUD pages with ADO.NET data entity model mapping and updating the database with the new schema. (Code below)

![ModelLiveProject2](https://user-images.githubusercontent.com/92835555/169889776-ccb315d2-5ebf-45b3-b4ac-8a2837c11905.PNG)
### User Story 3. * CRUD pages update create and edit pages with styling updates

- For this story I was tasked with updating the create and edit pages with styling updates to match the layout of the entire web app layout.  I updated these pages and changed the links into buttons for easy user navigation back to index page or to confirm/submit the form.  I also had to add a file based input to give user ability to choose a image file to add to their database from their machine. 
![LiveProject2CreatePgBefore](https://user-images.githubusercontent.com/92835555/169738489-65040c0f-697a-4963-9087-a136ed5e3191.PNG)
Create page before update (above)
Create page after update (below)
![LiveProject2CreatepgAfter](https://user-images.githubusercontent.com/92835555/169738498-372ce1d9-0e77-4465-99da-fd2ecc284636.PNG)
![LiveProject2EditPgBefore](https://user-images.githubusercontent.com/92835555/169738513-f0ac2dc4-5fb2-406e-a908-76d55382d38c.PNG)
Create page before update (above)
Create page after update (below)
![LiveProject2EditAfter](https://user-images.githubusercontent.com/92835555/169738507-6b0e71ee-4f40-4680-b0e1-6c0b44e4e901.PNG)



-  Second I was tasked to update the controller and index page to retrieve store and display images to the database and display all results on the index page.  This required storing the image as a byte[] in the database.  Within the create method I utilized HttpPostedFileBase class to take in the user file as a parameter and used the binary reader class to produce a byte[] for storage to database.  For display on the index the byte[] had to be converted into a 64base string and combined in the img tag.

![LiveProjectIndexBefore](https://user-images.githubusercontent.com/92835555/169738524-19cdc478-6e8a-4f5c-a6d1-55efb7a4ace6.PNG)
![IndexAfter](https://user-images.githubusercontent.com/92835555/169740203-a1481ec7-3940-43bf-b1b1-d2ca82827860.PNG)
![IndexSearch](https://user-images.githubusercontent.com/92835555/169740210-3f8471ee-45ab-4528-ac97-d0e45e9d1500.PNG)
![ControllerEdit](https://user-images.githubusercontent.com/92835555/169740525-f368d553-6132-4bef-89c9-62e7c9f14e3a.PNG)
![ControllerIndex](https://user-images.githubusercontent.com/92835555/169740532-33a27e75-2064-4d34-9275-0e8f219449d4.PNG)
![ControllerCreate](https://user-images.githubusercontent.com/92835555/169740541-c0b89b9c-cb83-4641-85c2-44c5ee4eb435.PNG)
![TextHelpersMethods2nd](https://user-images.githubusercontent.com/92835555/169887092-5667f8d9-8b6b-46cf-8c32-a17a594b1a2a.png)
