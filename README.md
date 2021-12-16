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

### Delete all class messages in `#class-selection`

Delete all messages that are posted in `#class-selection` EXCEPT the one at the very top for selecting your grade classification. 


## Create the new class list, channels and roles

### Login to the Digital Coffee account

You'll want to create the post in `#class-selection` using the Digital Coffee user account on Discord.   

If you don't know the username & password, ask the previous admin for it.


### Draft up the message that will be posted in `#class-selection`

Find the [full list of courses](https://prodssb.missouristate.edu/prod/bwckschd.p_disp_dyn_sched) being offered for the next semester.

Fill in a draft post of all courses being offered each semester. See [example.txt](https://github.com/alyaherron/digitalcoffee/blob/main/example.txt) for the formatting to use. 

Use your best judgement as to what classes to include. Typically this is all courses required to graduate with the Computer Science or Software Development degree, including the specific math requirements (calculus, statistics, etc.) and physics requirement.   


### Post it to `#class-selection`

Make sure you're logged into the Digital Coffee account, and then post the class messages in `#class-selection`. This needs to be broken up into multiple messages, separated by section (Intro Courses, Mid-Level Courses, etc.). 

Use [divider.gif](https://github.com/alyaherron/digitalcoffee/blob/main/divider.gif) in between each message.

### Edit roles for all the classes

Each class you have listed will need a specific role for it. In server settings, create new roles for all classes being offered, and delete any roles for classes that aren't being offered next semester. You can re-use roles that are previously there if the same class is offered again, but make sure all members listed under **Manage Members** are removed. All permissions for the role should be turned off. 

### Create new channels for each class

Each channel should allow channel access for Admin, Tutor, Retired Staff, and the role for that particular class. Here is an example for CSC 131:

![image](https://user-images.githubusercontent.com/59751268/146460750-d62d08e2-dd57-4bd5-a86a-0ff739786e38.png)

To make it easy on you, once you make the first channel, right click on it and select **Clone Channel**. All you have to do is rename it and update the permissions for the correct class role to view it. 


## Set up Carl-bot reaction roles

Carl-bot is the bot we utilize for allowing a message reaction to assign the user a role. 

### Login to Carl-bot

Head to [Carl-bot](https://carl.gg/) and login with your regular Discord account. You don't have to be logged into Digital Coffee's account for this part.

### Remove old reaction roles

Under your name at the top right, click **Servers**, and then click **Digital Coffee**. Under **Settings** on the left hand side, click **Reaction roles**.

Click edit & then delete for each one EXCEPT the one at the very top for grade classification reactions.

### Add new reactions for each message

Go to the class messages in `#class-selection`. Right click on the message for intro courses, and click **Copy ID**.

![image](https://user-images.githubusercontent.com/59751268/146459364-919a5698-2e2e-48d8-a8c3-567533cf7dbb.png)


Go back to Carl-bot, click **Create new reaction role**. 

Under **Mode**, select **Use ID**, and paste in the message ID. Select the `#class-selection` channel from the drop down.

![image](https://user-images.githubusercontent.com/59751268/146459585-8a0e48ac-2ffd-476c-b47e-c4d09f8c520d.png)

For each class you have listed in that particular message, add the corresponding emoji number, along with the class role.

![image](https://user-images.githubusercontent.com/59751268/146460251-15b78094-3ed5-4cb0-bfae-c48d79e10d05.png)

Repeat this process for each message in the channel.

![image](https://user-images.githubusercontent.com/59751268/146460419-c8471275-b1da-478b-8623-a5243b61f39d.png)

