Adam's dotfiles. Largely based on Simon Owen, but bits and pieces from all over the place.

Some important notes:
* Other people may find this useful, but it's mostly for me to use personally.
* The basic idea is that you put these somewhere handy (like your `code` directory), delete your dotfiles from the root of your user directory, then make symlinks there to these files via an install script.
* Edit the `install.conf.json` file to include/exclude the files you actually want to use.
* If you add more files, don't forget to reference them in line 8 of `bash_profile`
* Run the `install` bash script to create the links. The script first clears out any old symlinks, then makes new symlinks to the "undotted" versions of these files as dotfiles in your user directory.
* You only need to run the install script when you want to add/remove files. As you edit files, well they are symlinks so just does what you want.
* Take a look in the aliases file - there are some handy shortcuts in there that are only useful to me. You'll probably want to remove them or replace with your own.
* There are a couple of other personal configurations (default username in `bash_prompt`, name and email in `gitconfig`. Search for "adam" to be sure.
