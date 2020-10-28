# practiceDB dump file (mongodb)
# Jake Levy
# A simple dummy db assignment for students to practice with
# The starting point for the lab.  IF you were not in class or were otherwise
unable to follow along with the lecture activity, make sure you go back and
watch that video/get the notes from a fellow student, and do the exercises that
we do in the video, otherwise you will get "incorrect" results.  You'll be
turning in screenshots of your queries and transactions as well as their
results so I'll know if you were following along in the lecture. The insert
that I perform in the beginning should include your name and whatever other
info you want to share (you don't have to put your real email, if you don't
want to but it does need to be your name).

To setup the starting point for this lab, make sure your mongod service is
running. Make sure you are in THIS directory (lab 7) and then run:

	mongorestore --db=practiceDB dump/practiceDB
	^^		     ^^	      ^		^
	restore	    	  this DB     from this directory

WINDOWS USERS: you may need to download mongo database tools as a separate
package and then once downloaded and moved onto your harddrive,
specify mongorestore's full path (rather than just the command)


This assignment is relatively simple. Based on the stuff we did in the class,
the slides and notes you've been provided, and the MongoDB documents on query
(https://docs.mongodb.com/manual/reference/operator/query/) and update
(https://docs.mongodb.com/manual/reference/operator/update/) operators, perform
the tasks listed below in the practiceDB. It may take a few attempts to figure
each one out.

For the queries, once you have figured it out, take a screenshot of the query
and its result. For the update tasks, you should first figure out the query
by itself, or you may make a mistake in the update.  When finished all tasks,
upload all of your screenshots to correct Canvas link.
MAKE SURE THEY ARE REASONABLY LARGE ENOUGH FOR ME TO READ.  If I have to squint
to read the text, its getting marked incorrect.

IF you totally screw up and need to start all over, drop the database
(db.dropDataBase()) and then re-run the mongorestore at the top of this file.


1)  Write a query that will find the entry in users that contains your
information.  Any query that uniquely identifies your info is sufficient. Use
the pretty() command to make the result more readable.

2) Write a query that will find all records for "loc_the_viking" where distances are greater than or equal to 4.

3) Write a query that will find all activities with a distance greater than 5
OR less than 3.

4) Write a query that will find all activities for user heavyMetalHippy, where
the activity type value is "swimming"

5) Write a query to find all records with weights over 250 Use a projection
document to display only user, time, and distance fields (suppress everything
else)

6) Write a query that will find all records with activity type "running" but
returns only the _id and weight fields.

7) Write an update to change the email for _id: phreneticPhanatic to
levyj63@rowan.edu.

8)  Write an update that will set the weight for all activities with user:
heavyMetalHippy to 200.

9) Write an update that will find all entries for user grittyCity, that have
an activity type other than walking, and change them to walking.

10) Write an update that will find all activities where the user property has
NOT been set (aka it doesn't exist), and then set the user field for those records to be the _id value that corresponds to your entry in the users collection.
(HINT use the $exists operator)
