# Creating an MSc website using Netlify and Git

<h3> To set up your module website: </h3>
<br>
<b> Clone on Git: </b>
<ul>
<li>	Clone </li>
<li>  Copy link </li>
<li>	Create new repository </li>
<li>	Import repository </li>
<li>	Go to your new repository </li>
<li>	Copy the link to your repository </li>
</ul>
<br>
<b> Deploy on Netlify (to check it’s all working): </b>
<ul>
<li>	Create and/or log in to your Netlify account </li>
<li>	Connect it with your GitHub account </li>
<li>	Click ‘New site from Git’ </li>
<li>	Select the name of your new repository and ‘deploy’ </li>
<li>	Go to ‘Site settings’ and ‘change site name’ to the name you want to use </li>
<li>	The link with the site name should appear at the top left of the page, click this and see your new site! Copy the weblink </li>
</ul>
<br>
<b> Change the title of your site: </b>
<ul>
<li>	Start on your GitHub repository </li>
<li>	Go to /config/_default/config.yaml </li>
<li>	Edit (using the pencil icon on the right) </li>
<li>	Update the title and copyright you want to use, and paste the weblink under baseurl. (Be careful to keep any formatting, ie where there are quotations or not) </li>
<li>	Commit the changes </li>
<li>	Go back to Netlify >> Deploys and check it’s deployed correctly. Preview to see your changes. Do this after every update in Github, to spot any issues early </li>
</ul>
<br> 
<b> Change the Landing Page: </b>
<ul>
<li>	Go to /config/_default/params.yaml </li>
<li>	Edit the Contact section and the Twitter (under social) </li>
<li>	Check it Deploys correctly on Netlify </li>
</ul>
<br>
<b> Change the Intro box on the Landing page (stored in a widget so in a different location): </b>
<ul>
<li>	Go to content/home/hero.md </li>
<li>	Update the title and text </li>
</ul>
<br>
<b> Update the About page: </b>
<ul>
<li>	Go to content/about/index.md </li>
<li>	Edit to add the module details </li>
</ul>
<br>
<b> Update the Help page: </b>
<ul>
<li>	Go to content/help/index.md </li>
<li>	Edit to add the content </li>
</ul>
<br>
<b> Update the Timetable page: </b>
<ul>
<li>	Go to content/timetable/index.md (You can ignore the anchor files, these are just for the layout) </li>
<li>	On edit mode, you can see the three sections, which link directly to eg yourwebsite/reading/. If there is content for each session (making sure they have identical names), it will be populated under the respective heading here, on the live website </li>
<li>	The formatting content is saved under {{< schedule >}} which is a shortcode (short piece of html code. Edit under layouts/shortcodes/schedule.html) </li>
</ul>
 <br> 
<b> Update the Reading (or Labs or Homework) page: </b>
<ul>
<li>	Go to content/reading/_index.md </li>
<li>  Edit the content on Line 19 if you want new header text </li>
<li>  To edit a session, select the session file (eg content/reading/01-reading.md) and add content </li>
<li>	To create a new session, make sure it’s saved under content/reading, and copy the formatting from another session file for ease </li>
<li>	Once saved, this should appear both on the sidebar of the Reading page and also the grid on the Timetable page </li>
<li>	This is exactly the same process for the Labs and Homework pages (make sure the titles of each session are exactly the same for Reading, Labs and Homework) </li>
</ul> 
<br> 
<h3> Other things you might want to change: </h3>

<b> To update the cover image: </b>
<ul>
<li>	Upload the image to /assets/media and copy the file name, including extension </li>
<li>	Go to content/home/hero.md  </li>
<li>	Change hero media to the name of the uploaded file </li>
</ul>
<br>
<b> To update the icon (in the browser): </b>
<ul>
<li>	Upload a new icon.png to /assets/media </li>
</ul>
