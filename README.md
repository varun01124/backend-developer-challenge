Stagelink Backend Developer programming challenge
=================================================

Introduction
-----------

At Stagelink we strive to accurately measure and understand user engagement. Unfortunately metrics provided by Facebook like number of likes can be misleading and don't accurately represent overall fan engagement. We also like to identify and involve super-fans, who interact with artists and creators on a regular basis.

Therefore we build tools which are much better at understanding real fanbase and engagement on Facebook pages.

Your task is to create a tool which will collect Facebook IDs of users interacting with a given Facebook page.

Facebook users can interact with pages in multitude of ways:
- react to a post
- comment on a post
- tag person on a photo

In your solution you can use any means available to collect aforementioned information, be it Facebook API or direct page scraping.
However we would like to encourage you to use existing tools and solutions, especially those available on rubygems.org.

Input
-----

Solution should accept following input:
- list of IDs of Facebook pages
- number of latest posts to process

Below we provide a list of 3 example pages you can use for testing. Please keep in mind that the solution should accept any number of page IDs.

Output
------

Output should be provided as a CSV file in the following format

user_id, page_id, post_id, post_type, interaction_type [, interaction_subtype]

Example rows for my reaction and comment on the following Stagelink post would be
https://www.facebook.com/Stagelink/posts/1172918952749508

1278167270,305736219467790,1172918952749508,video,reaction,HAHA
1278167270,305736219467790,1172918952749508,video,comment

To complete the task you are required to list likes and comments. Photo tags are optional and you get extra points for implementing that.

Timeline & deliverables
-----------------------

You have up to a week to complete this task and provide a link to a Github repository including the code.
You can get extra points by showing your progress in git commit history.

Example input
-------------

305736219467790,10  
249403588440524,10  
107840939393927,15  

Useful resources
----------------

https://developers.facebook.com/docs/graph-api/reference  
https://developers.facebook.com/tools/explorer/

