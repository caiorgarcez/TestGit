This repository presents the basics of Git. A good reference for commands is found [here](https://www.youtube.com/watch?v=HVsySz-h9r4). 

-----

### Basic Tutorial 

First associate your Github account to your Git client: 
```shell
$ git config --global user.name "<enter here your username>"
$ git config --global user.email "<enter here your email associated to your Github account>"
```

A proper way for cloning your repositories and modify them is to create a folder called: ''Git'' at any directory of your choice.
```shell
$ mkdir <name of your directory>
```
In case of a new repository, navigate to the created directory by `cd /Git/<nameoftherepository>` and initiate the version control by: 
```shell
$ git init
```

Later, in the current repository, create and save a markdown file called ''README.md''. To verify the creation of the file, run the status:
```shell
$ git status
```

Notice that git warns about changes made in the repository. To confirm the  modifications run:
```shell
$ git add README.md
```

In case of more files. You can add them all by running:
```shell
$ git add --all
```

In case of clonning an existing repository, you can navigate to ''Git'' and run:
```shell
$ git clone <https://urloftherepository>
```
A folder will be created containing all the files of the clonned repository.

For pushing to Github the changes made in the repository, it is necessary to add a "commit tag message" to your files that are identified as modifications when running git status. In order to do so, run:
```shell
$ git commit -m "write here the commit" README.md
```

For a group of files, you can run:
```shell
$ git commit -am "<commit message for all modifications>"
```

Now you can publish on Github by running:
```shell
$ git push -u origin master
```

-----

### Allow Github to track a project repository at a local folder

Navigate to your local project repository and run `$ git init` to create a `.git` folder and start tracking the files. 

Access Github website and create a repository with the same name of your project's folder. After you finished the creation process, get the url of the repository and run:
```shell
$ git remote add origin https://github.com/<your_username>/<name_of_the_fodler>.git `
```

Your local project files will be added to your Github repository folder. Before commit, it is necessary to run: `$ git add --all
` to add the files. Later, run `$ git status` to make sure all modifications have been identified.

Then the commit the changes by: 
```shell
$ git commit -am "<Comment about adding repo to Github>"`
```

Push to Github by: 
```shell
$ git push -u origin master`
```

-----



