# Prog-II-Playground
This repository is created in the context of the Programming II course of the Department of Management Science and Technology and will serve as a playground for students to experiment with basic git and maven concepts.

## <a name="table-of-contents"></a>Table of contents
* [Git and GitHub](#git)
* [Maven](#maven)
* [Resources and Useful Links](#res)


## <a name="git"></a>Git and GitHub

**Git** is a popular version control system that enables changes tracking in projects and collaboration among developers.
**GitHub** is a code hosting platform that scales collaboration, by letting you contribute to software projects from anywhere.

This is a simple repository that you can use, in order to practice basic Git and GitHub projects. 
To begin with, you can clone this repository in your local system by using

``` 
  git clone https://github.com/apapadopoulou/Prog-II-Playground.git 
```

An alternative to the above approach is to create a git repository locally from scratch, add the remote repository and pull the files. 
When you pull the files from the remote origin repository, you should specify the branch from which you want to pull the files from. 
This will also enable your current local branch to track a specific remote branch.

``` 
  git init [name]
  cd [name]
  git remote add origin https://github.com/apapadopoulou/Prog-II-Playground.git
  git pull origin main
```

Another good practice when we want to collaborate in a project is to fork the initial remote repository at GitHub and create our own version.
To clone the newly created version locally, we will follow the aforementioned steps, of course changing the url of the repository where needed.
However, we need to add the main GitHub repository as upstream. This will help us fetch the changes from the main repository, to keep ours up to date.
The commands that do this are the following.

``` 
  git clone https://github.com/{your-username}/Prog-II-Playground.git
  git remote add upstream https://github.com/apapadopoulou/Prog-II-Playground.git 
```

> Note that these steps are mandatory if you want to publish changes into this project.

Now, let's experiment! You can contribute to this project by creating a fork, make changes in a new or in an already existing branch and create a pull request.
Remember that when you make a change in a file, you should execute the following commands to commit it.

```
  git add [changed-file]
  git commit -m [message]
```

Remember to always use descriptive messages in your commits. When you want to push your changes at GitHub, you use

``` 
  git push origin [branch-name] 
```


## <a name="maven"></a>Maven

**Maven** is an open-source tool that enables building, publishing and deploying applications, offering efficient software project management.
It comes with a large list of benefits for software developers, with the most important of them beign dependency management, and can help you scale your projects, by following the field's best practices. 

After downloading and configuring Maven (the instructions can be found in the Apache Maven [website](https://maven.apache.org/what-is-maven.html)), you can begin by creating a pet project to experiment with. You can follow the instructions [here](https://www.simplilearn.com/tutorials/maven-tutorial/maven-project-in-eclipse), in order to create a project from scratch.

In addition, we have created a simple maven project in the branch `add-maven`. You  can import this project in Eclipse and the rest is up to you! 
You can add classes, tests and methods for extra functionality and see how everything connects using Maven. Feel free to alter the `pom.xml` file and use external libraries in the existing or in new classes. See that when you execute `mvn clean package` at the directory that contains the POM file,
the libraries are automatically installed in your system.


## <a name="res"></a>Resources and Useful Links

- [Git Download and Documentation](https://git-scm.com/)
- [Git Cheat Sheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)
- [Maven Download and Documentation](https://maven.apache.org/)
- [Maven Plugins](maven.apache.org/plugins/index.html)
- [Maven Repository](https://mvnrepository.com/)
- [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)
- [Commit Messages Best Practices](https://initialcommit.com/blog/git-commit-messages-best-practices)
