# dsus

Creating an MSc website using Netlify and Git

To set up your module website:

Clone on Git:
	Clone
	Copy link
	Create new repository
	Import repository
	Go to your new repository
	Copy the link to your repository


Deploy on Netlify (to check it’s all working):
	Create and/or log in to your Netlify account
	Connect it with your GitHub account
	Click ‘New site from Git’
	Select the name of your new repository and ‘deploy’
	Go to ‘Site settings’ and ‘change site name’ to the name you want to use
	The link with the site name should appear at the top left of the page, click this and see your new site! Copy the weblink.








Change the title of your site:
	Start on your GitHub repository
	Go to /config/_default/config.yaml
	Edit (using the pencil icon on the right)
	Update the title and copyright you want to use, and paste the weblink under baseurl. (Be careful to keep any formatting, ie where there are quotations or not)
	Commit the changes
	Go back to Netlify >> Deploys and check it’s deployed correctly. Preview to see your changes. Do this after every update in Github, to spot any issues early. 

Change the Landing Page:
	Go to /config/_default/params.yaml
	Edit the Contact section and the Twitter (under social)
	Check it Deploys correctly on Netlify

Change the Intro box on the Landing page (stored in a widget so in a different location):
	Go to content/home/hero.md
	Update the title and text
Update the About page:
	Go to content/about/index.md
	Edit to add the module details

Update the Help page:
	Go to content/help/index.md
	Edit to add the content

Update the Timetable page:
	Go to content/timetable/index.md (You can ignore the anchor files, these are just for the layout)
	On edit mode, you can see the three sections, which link directly to eg yourwebsite/reading/. If there is content for each session (making sure they have identical names), it will be populated under the respective heading here, on the live website
	The formatting content is saved under {{< schedule >}} which is a shortcode (short piece of html code. Edit under layouts/shortcodes/schedule.html)

Update the Reading (or Labs or Homework) page:
	Go to content/reading/_index.md
	Edit the content on Line 19 if you want new header text 
	To edit a session, select the session file (eg content/reading/01-reading.md) and add content
	To create a new session, make sure it’s saved under content/reading, and copy the formatting from another session file for ease.
	Once saved, this should appear both on the sidebar of the Reading page and also the grid on the Timetable page
	This is exactly the same process for the Labs and Homework pages (make sure the titles of each session are exactly the same for Reading, Labs and Homework)

Other things you might want to change:

To update the cover image:
	Upload the image to /assets/media and copy the file name, including extension
	Go to content/home/hero.md 
	Change hero media to the name of the uploaded file

To update the icon (in the brower):
	Upload a new icon.png to /assets/media
