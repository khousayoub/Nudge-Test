# Steps to install my project on localhost : 
• Install DDEV
• Create a new directory
• Go to this directory and execute this commande : `ddev config --project-type=drupal9 --docroot=web –create-docroot`
• modify the route ports in the file that is in the project directory: `.ddev/config.yaml` :
		◦ router_http_port: from "80" to "8880" for example
		◦ router_https_port: from "443" to "9443" for example
• execute these commands :
	```
	ddev start
	ddev composer create "drupal/recommended-project"` ("yes" to clear the directory)
	ddev composer require drush/drush`
	ddev import-db –src={the/dump/path}/db.sql.gz
	```
• For the last step beofre launching the project, copy all the files from my project folder into your directory and execute this command : `ddev launch`

# Technical questions : 
1. How long did you spend on the coding test? I spend around 2 days, average of 6/7 hours per day,it's about 12/14 hours.
2. What would you add to your solution if you had more time? If I had more time I would add :
	1. Change the theme and add more styles on my web site. 
	2. I would also add more advanced search featers such as : Facets, I tried to experience it but it seems a little bit complicated and take a lot of time so I decided to focus on the exercise instead of it.
	3. Add more pages and manage more blocks such as the header, menus, footer and sidebars.
3. How would you ensure that this application could be efficiently extended and maintained by a small team of developers over time?
	1. Update the developement environement and each libraries/modules/themes that we use in the application in order to keep our application secure.
	2. code properly, it means that the coder should follow the good practices in coding so the next coder who going to take back the code can easily understand it and continu on the same way.
4. What quality assurance checks should be performed as part of further application development? 
	2. put lot of a code comments especialy when there is a part which is a bit complicated.
	3. write a technical and functionnal documentation about this application/web site. 
5. How would you approach debugging a reported issue in the application?
In order to debugging application we need the test tools, so it makes debugging very efficient and clear and we can save lot of time.Sometimes we cannot solve the issues whithout checking the "troubelshooting" sections that the coder community offer, sometimes it inevitable. After debugging the application and fix the issues, the coder should write every steps that he did in the technic documentation, so if someone else who works in the project got the same issue, he can "save his life", maybe he can spend days to trying to solve the problem.

# Passwords : 
Admin account : 
	user : ayb
	password : ayb
Other account :
	user : contributor
	password : azerty

# Feedbacks about the test : 
I would like to mention some points about the test that maybe you can add it to the future tests :
	1. I would like to add to the test : adding the project into a git repository so you can see how long the tester worked on his project and how many commits did he, and maybe ask them to wokr on different branchs depending on featers for example : create branch to make the search feater. I think that every developer team works with those versionning tools (github, gitlab or bitbucket) so it's good to evaluate the candidate on this point.
	2. Also you can give the candidate the freedom to host his application in a hosting site unless if you dont want to for your own reasons.
	3. Add more featers regarding to other users such us creating new users and give it some different permissions.
