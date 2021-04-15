# samsick.github.io
Built angular app to be deployed on github. This app will give you important informations of the ctrlX Automation Community.<br>

Relevant data from the ctrlX AUTOMATION community is to be queried via the interface and processed in a suitable form. Furthermore, a write access to the community from this web interface shall be enabled e.g. to reply to certain forum posts, create new posts, etc. The standard REST interface supplied by Khoros is used for this purpose (https://developer.khoros.com/khoroscommunitydevdocs/reference/khoros-communities-platform-apis). <br><br>
Important data of the community can be e.g. the following: users, posts or tags. 
There is a dashboard for a general overview as well as individual pages for each of the three points mentioned above. The design is kept consistent across all pages, so only the actual content changes. The dashboard is used as an example to illustrate the interface: <br><br>

![Community Overview Dashboard](src/assets/community_overview_dashboard.png)

According to the current status, the following functionalities are provided on the individual pages:
* User: Shows all users sorted alphabetically with username, number of posts, profile picture, online status and offers a search option to search for all posts of a specific user
  * Screenshot of the user overview:
![Community Overview Dashboard](src/assets/user_overview.png)
  * Screenshot of an opened post in the posts per user overview:
![Community Overview Dashboard](src/assets/posts_per_user_opened.png)
* Posts: Displays the latest posts in the community (no replies) and provides a search option to look for specific posts
  * Screenshot of the post overview:
![Community Overview Dashboard](src/assets/latest_posts.png)
* Tags: Displays all tags of the community (sorted alphabetically, with weighting) and offers a search option to search for entries with specific tags and tag combinations

## How to install and run the project
When installing and running the project, it is assumed that node.js is already present on the respective computer (Download here: https://nodejs.org/en/download/). <br><br>
First, the project must be cloned to a local directory on the device. Then you need to navigate to this directory using the console and execute the following command:<br>
```
npm install
```
This will install all the required dependencies for the project and it's ready to go. To start Angular's Live Development Server and therefore also the web project, you need to execute either the command
```
npm start
```
or if you already downloaded the CLI (Command Line Interface from angular)
```
ng serve 
```

The project listens by default on localhost:4200, so you only need to enter this adress in your browser to see the correspondending web interface. <br><br>
Each time a change is saved, the page is reloaded and the updated result is displayed.


## Helpful links
* Khoros REST API description: <br> https://developer.khoros.com/khoroscommunitydevdocs/reference/khoros-communities-platform-apis 
* LiQL collection: <br> https://developer.khoros.com/khoroscommunitydevdocs/docs/liql-collection-reference


