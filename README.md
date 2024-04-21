# rikon

My personal file collectors and backup service.

This project solves a very simple problem that I have with a simple workflow as follows:

1. I have a folder that contains mainly text files, e.g., some code snippets, logs, and notes.
2. I want to update and back up them with git.
3. I shouldn't do step 2 manually. Based on some time frequency or amount of changes, it stages the changes, creates a commit, and uploads to GitHub.
4. The services should be a daemon process.
5. It should ask me some very basic questions to set up but nothing more.
6. Finally, I can monitor the folders that I sync with it, can edit and remove the path.

The tech stack seems very simple as well:
1. watchdog library to watch the changes
2. using shell utilities to control git
3. docker to package as a services
4. a small web protocol to fill in the information / simply some config file will do when setting up.
