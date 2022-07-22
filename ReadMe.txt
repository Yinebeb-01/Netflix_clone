              ***
***Netflix Clone by using Django***
      By: Yinebeb Tariku, ETS1263/10
              ***
=>files in this zip folder(I listed only the mains(important one)):
	-django_netflix - the directory created when the admin start the project django_netflix. It contains configuration files 
		like asgi.py,settings.py,urls.py,__iniy__.py and wsgi.py.
	-core -this directory is the app that is the main part of the whole project. It contains __init__.py,admin.py,apps.pyforms.py,
	 	models.py, urls.py and views.py.
	-media - this directory is used to store files those are uploaded to the clonned-site, like movies, videos and flyers.
	-static - this directory contains static files like html files, and related stylesheets including images and related icons..   
	-templates - this directory contians tempaltes used in the project such as base.htm and index.html files.
	-db.sqlite3 - this databse file is used to manage and store the whole database fro the project.
	-manage.py - this python file is used to manage command line operations such as running and manipulating the project from 
		a cmd,specially for adminstrative tasks.
	-requirements.txt - text file which consists of the required packages list need to installed for the project before testing/running.

=>The project is all about clonning Netflix webapp by using pyhton's rapid web framework-Django.
Netflix is video streaming weapp.

=>NB: If you want to test by running, ensure the virtual environment is installed well. And for no clue, my testing Chrome browesr can't render  the html and css file 
	as expected and I was doing on the Microsfot Edge browser. So use Microsoft Edeg when you run the server to see the cloned webapp.

=>A bit detail description:

=>In the model.py files, there are profile, customer,movie and video tables(or collections) along their attributes.
 -Customer is an abstractuser, inheriting attributes from the django user like name and password. It has many to many 
	relationship with profile.
 -Profile have attributes of name,age_limit(for kid vs all), and universal unique identifier(uuid).
 -Movie have attribute title,description,created date,uuid,type(single vs seasonal), flyer and age_limit.
 -Video have attribute title and file. Many to many relationship is created between movie and video.
*A user-here a customer need to signup and registered with his email address along a strong password. 
 Once he/she sign up, he can create upto five profiles. Profiles are just an instantiate of the genuin table 
 Customer. Here it is used as a table favorites to store and save their subscriptions and video history in 
 an organized manner. 
*An admin(super user) can add videos, movies and manage other adminstrative tasks by navigating to localhost/admin page.
 -Users can logged in and see videos/movies on their profiles. 
 -Movies and videos are uploaded with a description notes which tell user an info about it and comes with a flyer.

=> As I mentioned above, a user can have upto five profiles(just the number is optional) and when a user create a profile,
for the type of the subscripton he want, there should have an uploaded videos for that type ,kids or all. so for the first 
	time ensure you have a video for both options.
=> In the bottom section of the webapp I added footer having a copyright, project name and my name-clickable which navigate to a page about myself(about.htm).

=>Due to the rushing time and other project load, I tried to incorporate only these features.

*** The end ***