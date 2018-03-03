### TestGit
This a repository made for testing Git. 

-----

### Some useful commands 

The first step is to create a folder called: ''Git'' for cloning your repositories and modify them. 

Later, it is necessary to associate your Github account to your Git client. 

`$ git config --global user.name "enter here your username."`

`$ git config --global user.email "enter here your email associated to your Github account."`

Then clone the repository in your created Git folder.

`$git clone https://urloftherepository.`

Create a markdown file called myfistfile.md. The objective is to add this file to your Github repository. Then run:

`$ git add myfirstfile.md`

In order to verify the creation of the file, run the status.

`$ git status`

Add a commit to your file.

`$ git commit -m "write here the commit" myfirstfile.md`

Now you can publish on Github by running:

`$ git push -u origin master`

-----
