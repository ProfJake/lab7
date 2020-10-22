# practiceDB dump file (mongodb)
# Jake Levy
# A simple dummy db for students to practice with
# The starting point for the lab.  IF you were not in class or were otherwise
unable to follow along with the lecture activity, make sure you go back and
watch that video/get the notes from a fellow student, and do the exercises that
we do in the video, otherwise you will get "incorrect" results.  You'll be
turning in screenshots of your queries and transactions as well as their
results so I'll know if you were following along in the lecture.

To upload the starting point for this lab, make sure your mongod service is
running. Make sure you are in THIS directory and then run:

	mongorestore --db=practiceDB dump/
	^^		     ^^	      ^^
	restore	    	  this DB     from this directory

This assignment is relatively simple. Based on the stuff we did in the class,
the slides and notes you've been provided, and the MongoDB documents on query
(https://docs.mongodb.com/manual/reference/operator/query/) and update
(https://docs.mongodb.com/manual/reference/operator/update/) operators, perform
the tasks listed below in the practiceDB. It may take a few
attempts to figure it out.  For the queries, once you have figured it out,
take a screenshot of the query and its result. For the update tasks, you should
first figure out the query by itself, or you may make a mistake in the update.

IF you totally screw it up and need to start all over, drop the database and
then re-run mongorestore. 
