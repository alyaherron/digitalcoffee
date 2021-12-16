# Class Selection Bot

TLDR;
- x
- y
- z


## Turn off view permissions for `#class-selection`

Before doing anything, we need to prevent people from getting spammed with notifications. 

Head to the settings of `#class-selection` and click the **X** next to **View Channel** for the **@everyone** role. 

Keep the **ADMIN** role turned on, but give a heads up to `#admin-only` to ignore any notifications they get from the channel. 


## Delete erry-thang


### Edit the Flavors category

Change the `Flavors - [semester][year] Courses` category name to the new semester & year.

### Delete all the current course channels

Even if the course is being offered again next semester, it's necessary to delete it so that the messages are purged. 

### Delete messages in `#class-selection`

Delete all messages that are posted in `#class-selection`. 


## Create the new class list and roles

### Login to the Digital Coffee account

You'll want to create the post in `#class-selection` using the Digital Coffee user account on Discord.   

If you don't know the username & password, ask the previous admin for it.


### Draft up the message that will be posted in `#class-selection`

Find the [full list of courses](https://prodssb.missouristate.edu/prod/bwckschd.p_disp_dyn_sched) being offered for the next semester.

Fill in a draft post of all courses being offered each semester. See [example.txt](https://github.com/alyaherron/digitalcoffee/blob/main/example.txt) for the formatting to use. 

Use your best judgement as to what classes to include. Typically this is all courses required to graduate with the Computer Science or Software Development degree, including the specific math requirements (calculus, statistics, etc.) and physics requirement.   


### Post it to `class-selection`

Make sure you're logged into the Digital Coffee account, and then post the classes message in `#class-selection`.  

### Edit roles for all the classes

Each class you have listed will need a specific role for it. In server settings, create new roles for all classes being offered, and delete any roles for classes that aren't being offered next semester. You can re-use roles that are previously there if the same class is offered again, but make sure all members listed under **Manage Members** are removed. All permissions for the role should be turned off. 

## Set Up Carl-bot Reaction Roles

Carl-bot is the bot we utilize for allowing a message reaction to assign the user a role. 

### Login to Carl-bot

Head to [Carl-bot](https://carl.gg/) and login with your regular Discord account. You don't have to be logged into Digital Coffee's account for this part.

### Add reaction roles

Under your name at the top right, click **Servers**, and then click **Digital Coffee**. Under **Settings** on the left hand side, click **Reaction roles**.
