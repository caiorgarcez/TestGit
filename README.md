### TestGit
This repository presents the basics of Git. 

A good reference for commands is found [here](https://www.youtube.com/watch?v=HVsySz-h9r4). 

-----

### Some useful commands 

The first step is to create a folder called: ''Git'' for cloning your repositories and modify them. Go to any directory of your choice and run in Git Bash: 
`$ mkdir  Git"`

Later, associate your Github account to your Git client: 

`$ git config --global user.name "enter here your username"`

`$ git config --global user.email "enter here your email associated to your Github account"`

Then clone the repository of your choice in your recently created Git folder.

`$git clone https://urloftherepository.`

In case of a new repository, navigate to the created directory using `cd /nameoftherepository` and insert a markdown file called README.md:

`$ git add myfirstfile.md`

In order to verify the creation of the file, run the status.

`$ git status`

For pushing to Github changes in the repository, it is necessary to add a "commit tag message" to your files that are identified as modified when running git status. To do so, run:

`$ git commit -m "write here the commit" myfirstfile.md`

Now you can publish on Github by running:

`$ git push -u origin master`

-----
