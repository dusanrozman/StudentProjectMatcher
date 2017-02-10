# StudentProjectMatcher

# Description
This was an academic project that was created by Myself and two other students. The application is meant to solve the age old problem of placing students into groups/teams for group projects. The application allows Administrators (Professors) to create a project and allow student users to join the project. The students have the ability to change a variety of attributes in their profile to best mirror their skills and allow them to indicate what an ideal project partner would be for them. Once students are registered an Administrator can go ahead and run the CUPID algorithm which sorts students as best as possible based on their preferences.

The Application was made using C++ and QTCreator for the GUI portion. 

# How to run the project:
 - Import project using 'cuPIDapp.pro' file in the 'cuPIDapp' folder using QT on the COMP3004 VM.
 - Compile
 - *IMPORTANT* After compiling the program you should have a folder called 'build-cupIDapp-Desktop-Release'. the cupid_new.db provided needs to be manually placed in here. 
 - Run the program.

# How it works:
  - Once you run the program a login window will appear:
  - You can sign in as either an Admin or as a Student
  - There are already 25 student accounts and a few admin accounts
  - Select your username and select whether you are an admin or student using the radio buttons
  - The names are case sensitive so "Alice" and "alice" are different if you sign in with "Alice" alice already exists and is registered."alice" however will create a new student account called 'alice' 

# Use any of these student or admin names:

    | Accounts 	| Students  |	Admins |
    |--------- 	|:--------:|    ------:|
   |		| Alice	|	Admin1	|
	| | Bob		|	Admin2	|
	| | Charlie	|	Admin3	|
	| | Peter	|		|
	| | Susan	|		|

For testing purposes the passwords are all 'p'
Once you log in the rest should be simple.
# the Admin Menu/Profile window:
- Once you log in to an Admin account, you'll be in the Admin profile window
- Everything should be blank to start with except 'My Project' box (unless  you signed into a new Admin account).
- Click the project you wish you select (ie, "Admin 1's Project") and hit the select button
- You'll notice the 'update/view project' data gets filled out on the right. You can edit things like team size and project name there... 
- After you 'hit select' Student's registered in the project should appear in  the registered students window
- There are no teams created to start off with so teams in project and team roster should be empty.
- To create teams Select the project from 'My Project' window and hit 'Run PPID'
- The 'Teams in Project' window should now show teams.
- Select a team from 'Teams in Project' list and it will show the students on that team
- Other than that on the far right you can also create new projects. Just fill in the fields  and hit create. Note that "Project ID" is not necessary at the moment. It was meant  to be used for our database.
That's it for admin menu!

You can now exit and Admin Menu and log in as a student (say 'Alice' for example).

# Student Menu/Profile:
- First thing you will notice on the right is your profile. You can set the valuesto whatever you want and click update. These determine how a student is matched.
- On the left you should see a list of all Admins filled out.
- If you *double click* on an Admin there project will either appear in "Registered In" window or "Projects Not Joined". In this case Alice is in all the pre-made projects for Admin1, Admin2, Admin3.
- If you double click a project from the "Registered In" project will show you the team you are on and fill out the roster information. Of course that's IF you already ran the PPID algorithm (otherwise no one is on a team).
- If there is a project that a student is not registered in it will appear in the 'Projects Not Joined' window (after an Admin is selected). You can selected one of those projects and click 'Join Project' to join. 

That's essentially it!
