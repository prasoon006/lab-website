## Steps to add data

### Add Images

The images specific to items such as profile image of a author, project or talk image will go to the specific folder of that item. The name of image for the author should be "avatar" with .png or .jpg extension. For events and projects name should be featured with .png or .jpg extension. 
Images used in the website such as background images or logo or icon will go to /static/media and /assets/media/ both the folders. 



### Add Content

#### All the important/required content is avaiable in /content folder which include following folders :-

/author -> This folder contains folder for each team member with their names. The admin folder is of Prof Naomi Keena. Each folder contains two files, one is avatar.png, the profile picture of the team member, second one is _index.md which contains all the information about that member.   
To add any new team member just copy paste the complete folder of any author, and change the content inside it accordingly.  

/event , /project , /publication , /opportunities -> This folder contains list of all the respective Items. To add any other Item, just copy paste any of the previous indivisual item and change the content of copied item respectively. 
For opportunities, the current no-opportunity is also a indivisual item, so if you need to add a opportunity, copy this No-Opportunity folder and edit the copied folder accordingly and then delete the previous folder.

/home folder contains the items which needs to be displayed in the home page. demo.md , demoNext.md and demoPrev.md are displayed on the home screen. The actual size is given inside of these folder. 



### Building the Site locally

Step-1 : Install hugo on your system, you can find steps in the below article. 
https://thenewstack.io/tutorial-use-hugo-to-generate-a-static-website/

Step-2 : Clone the repository
command git clone https://github.com/McGill-TRACE-lab/TRACElab-website.git
Make sure you are the owner or have access to this repository. 
If still you are not able to clone, try this command  git clone https://yourgithubusername@github.com/McGill-TRACE-lab/TRACElab-website.git

Step-3 : After cloning, move inside TRACElab-website folder. 

Step-4 : Run hugo server, if you have installed hugo succesfully, you can see the website running on the port 1313. http://localhost:1313

Make any changes you want, you can see the live changes in the website on the port 1313. 



#### If you face below mentioned error

failed to resolve output
it says Error: from config: failed to resolve output format "WebAppManifest" from site config. I found the solution here. However I could not find any temp directory. Here is my solution:

Temporarily remove the “WebAppManifest”, “redirects”, “headers” output types from your config.yaml under the config folder (not the root folder) and run the following commands through Windows PowerShell: "hugo mod clean" and "hugo mod tidy"
Check that hugo now runs OK with "hugo server" or blogdown and then add the output types back into your config.yaml.

More troubleshooting solutions and complete steps to run the site locally are given in this article. https://thenewstack.io/tutorial-use-hugo-to-generate-a-static-website/

If you face any other issues with hugo, try updating hugo with command "hugo mod get -u".


 







