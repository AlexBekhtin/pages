### hg log - How to get the last 5 log entries?

Use the limit parameter: `hg log --limit 5`


In completion of the Michael Markert response you can use the shortversion

`hg log -l 10`

In addition if you want you can define via the option -b that you want only last commit from the current branch.

You can also do

`hg log -l 10 -b [your branch]`

for check 10 last commit from the branch you want

Of course you can go further with -d like this :

`hg log -l 1 -d "feb 2015 to apr 2015"`

This will give you last 10 commits within this date range (3 char for each months)

And goes on..

Full example and option are available in this link : Here

https://stackoverflow.com/questions/6835511/hg-log-how-to-get-the-last-5-log-entries
