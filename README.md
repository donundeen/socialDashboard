# socialDashboard
A webpage/server combination that renders a nice-looking view (or views) of social media streams, based on entered search criteria.


NOTE: This software doesn't have any "moderation" feature. Matching tweets, Instagrams pics just go up on the screen. So the utility of this tool is limited to areas where that is ok. Ideally at conferences with very specific hashtags, and a generally civil membership.

NOTE: Instagram policies have changed, so currently this tool works ONLY with twitter. working on a fix...


How to Use:
- clone into a directory on a web server
- copy secrets.tpl.js to secrets.js
-- add your twitter and instagram API keys
-- set the port values
- run "node server.node.js"
-- keep "npm install"-ing missing modules until it runs
-- (TODO: make a package.json file)
- open a browser to the server address and port
- the default search terms are "metmedialab" and "metmuseum"
-- hovering your mouse in the upper left corner reveals a gear icon. click on it to open a menu that will allow you to set your own search terms. Click the checkbox and it will resume with your new terms.
- you can call with url params
-- searchterms : comma-separated list of words to search in social media for.
-- fontsize: one of 'small','normal','large','jumbo'

TODO
- more options in menu, for color, size, etc
- option to clear all items 
- save values when iterface is closed.
