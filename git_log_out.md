> Remove your SSH keys from ~/.ssh (or where you stored them).

> Remove your user settings:
```
git config --global --unset user.name
git config --global --unset user.email
git config --global --unset credential.helper
```
> Or all your global settings:
```
git config --global --unset-all
```
Maybe there's something else related to the credentials store, but I always used git over SSH.

## addition
Git itself (the command line client, i.e. the ["stupid content tracker"](https://git-scm.com/docs/git) has no notion of user names, only GitHub does. 
In other words: there is no mapping of GitHub usernames to author/committer names and e-mails stored in a Git repository.


When creating a commit with Git it uses the configuration values of user.name (the real name) and user.email (email address). 
Those config values can be overridden on the console by setting and exporting the environment variables GIT_{COMMITTER,AUTHOR}_{NAME,EMAIL}.

Git doesn't know anything about GitHub's users, because GitHub is not part of Git. 
So you're only left with an API call to GitHub (I guess you could do that from the command line with a little scripting and make that a [Git alias](https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases).



https://stackoverflow.com/questions/7552054/git-cli-get-user-info-from-username

https://stackoverflow.com/questions/28238037/git-log-out-user-from-command-line
