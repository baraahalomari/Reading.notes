Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
Version Control is a system: that allows you to revisit various versions of a file or set of files by recording changes.


"Git mostly relies on local operations because most necessary information can be found in local resources, This allows for process expediency because a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work on a project even when not online"


Every time we change applied to any file is tracked by Git, and minimize the possibility of irreversible damage to files, such as accidentally lost data.

I learned how to To import an existing project or directory into Git by use the git command after cloned the file and create a copy of an existing Git repository from a particular server,

$ git clone URL
$ git add .
$ git commit -m “any message here”

to see information regarding changes to be committed use the git status command

$ git status

Finally you would push changes to a remote repository
$ git push origin main