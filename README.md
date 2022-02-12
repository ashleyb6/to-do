# to-do

Description:

A simple to-do list app that allows you to add tasks, 
'check' when done, and replace completed tasks with new ones.
The app allows users to have up to 8 tasks on their to-do list, 
but beyond that they must complete tasks before adding more.

Developed using Python 3.10 in PyCharm, 
using the tkinter package to design my interface. 

====================

Functions:

add_item()
  - add new items to list
  - append to end of list if less that 8 items, otherwise 
    replace first found completed item
  - send warning if there are 8 incomplete items in list
  
complete_task()
  - loop through buttons, replace 'incomplete' button with 'complete' button 
    if it matches the location where the button was clicked
    
=====================

Hardest part(s):

Figuring out the logic of replacing already completed tasks within add_item().
I found that when I added an image into a print statement, they each had a different 
name. The 'completed' image is called pyimage2. Using that knowledge, I decided to add 
all buttons to a list as tasks were added so I could loop through, tap into each buttons 
'image' attribute, and if it matched the name of the 'completed' icon, it would be replaced 
with the new task and an 'incomplete' icon. I also adding a boolean variable called 'keep 
checking' to exit the for loop once a completed item was found, to ensure all completed items would 
not be replaced.


