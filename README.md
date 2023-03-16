# Splunk-using-fields-elearning
Course : Using Fields (eLearning with labs)

Impossibiliy is Nothing!
It great to have completed the @VTF DAY 2 Bootcamp Security Analyst Training
Day 2. - https://education.splunk.com/course/using-fields-elearning
Course : Using Fields (eLearning with labs)

Below are the highlights of the course.

* Using the Fields Sidebar
 	- SELECTED FIELDS
	- INTERESTING FIELDS

* Using Fields in Search
  some commands used:
	fields
	stats count
	rename
	sort
	table
	erex
	rex

Lab Exercise 1 – Using Fields in Searches

Task 1 - Log into Splunk and change the account name and time zone.
Set up your lab environment to fit your time zone. This also allows the
instructor to track your progress and assist you if necessary.

Task 2 - Use the Fields sidebar to examine search results
Search online sales data (index=web sourcetype=access_combined) for all events containing a
purchase action (action=purchase.) Execute this search over the Last 24 hours.

Task 3 - Compare results from searches using the !=, NOT, and =* field expressions.
Search for index=web sourcetype=access_combined with a time range of Yesterday.
How many events are returned?  


Task 4 
Scenario: SecOps wants a list of authentication failure events associated with admin roles over the
last 60 minutes.

Search the web server (index=security sourcetype=linux_secure) for events during the Last 60
minutes.
Modify your search to look for:
a. Failed password attempts by invalid users by adding failed invalid to your basic search.  
b. Events associated with the administrator user, i.e. user accounts that begin with admin.   


Task 5 - Complete the missing portion of a search with the rename command.

This search finds purchase events from the online sales data that encountered a server problem
(status>399.) Complete the <missing> portion of this search so that the clientip field is renamed to
"Customer IP", the host field is renamed to "Web Server", and the status field is renamed to "HTTP
Status." Run this search over the Last 4 hours.


Lab Exercise 2 – Comparing Temporary vs Persistent Fields

Task 1
Scenario: SecOps wants to see a count of event descriptions by port from all web server events over
the past 7 days.

Use the erex command to extract temporary fields and include events based on pattern
matching.

Task 2
Use the rex command to improve your search results from Task 1.


About uploading data
When you add data to your Splunk deployment, the data is processed and transformed into a series of individual events that you can view, search, and analyze.


What kind of data?
The Splunk platform accepts any type of data. In particular, it works with all IT streaming and historical data. 
The source of the data can be event logs, web logs, live application logs, network feeds, system metrics, change monitoring, message queues, archive files, and so on.


Where is the data stored?
The process of transforming the data is called indexing. 
During indexing, the incoming data is processed to enable fast searching and analysis. 
The processed results are stored in the index as events.

The index is a flat file repository for the data. For this tutorial, the index resides on the computer where you access your Splunk deployment.

Events are stored in the index as a group of files that fall into two categories:

Raw data, which is the data that you add to the Splunk deployment. The raw data is stored in a compressed format.
Index files, which include some metadata files that point to the raw data.
These files reside in sets of directories, called buckets, that are organized by age.

By default, all of your data is put into a single, preconfigured index called main. 
You can create indexes to store your data when you add the data to your Splunk instance. 
There are also several other indexes used for internal purposes.

https://education.splunk.com/award/completion/34287e10-22b5-3544-83b9-bf58c469b1b9/view-ext


Author: Sabur Olamilekan Yinus | sabur.yinus@gmail.com
