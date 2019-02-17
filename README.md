This repository presents the basics of Git. A good reference for commands is found [here](https://www.youtube.com/watch?v=HVsySz-h9r4). 

-----

### Useful commands 

The first step is to create a folder called: ''Git'' for cloning your repositories and modify them. Go to any directory of your choice and run in Git Bash: 
```Linux Kernel Module
$ mkdir <name of your directory>
```

Later, associate your Github account to your Git client: 
```shell
$ git config --global user.name "<enter here your username>"
```

```shell
$ git config --global user.email "<enter here your email associated to your Github account>"
```

Then clone the repository of your choice in your recently created Git folder.

`$ git clone https://urloftherepository.`

In case of a new repository, navigate to the created directory using `cd /nameoftherepository` and insert a markdown file called README.md:

`$ git add myfirstfile.md`

To verify the creation of the file, run the status.

`$ git status`

For pushing to Github the changes made in the repository, it is necessary to add a "commit tag message" to your files that are identified as modified when running git status. In order to do so, run:

`$ git commit -m "write here the commit" myfirstfile.md`

Now you can publish on Github by running:

`$ git push -u origin master`

If you have uploaded/created files, before pushing to origin, you can add and commit all files with the following command:

`$ git add -A && git commit -m "write here the commit"`

-----

### Allow Github to track a project repository at a local folder

Navigate to your local project repository and run `$ git init` to create a `.git` folder and start tracking the files. 

Access Github website and create a repository with the same name of your project's folder. After you finished the creation process, get the url of the repository and run:

`$ git remote add origin https://github.com/<your_username>/<name_of_the_fodler>.git `

Your local project files will be added to your Github repository folder. Before commit, it is necessary to run: `$ git add --all
` to add the files. Later, run `$ git status` to make sure all modifications have been identified.

Then the commit the changes by: `$ git commit -am "<Comment about adding repo to Github>"`

Push to Github by: `$ git push -u origin master`

-----



