# Activity 2

> During this activity, it's possible that some of you may encounter difficulties with GitHub authentication. This presents an excellent opportunity for group collaboration and an initial step in problem-solving, as you'll soon be developers. Part of the learning process involves learning how to seek solutions.

These activity is designed to help you install and configure Git,  create a Markdown README.md file, and a GitHub repository:

### Task 1

In this task, you will install Git, configure it with your name and email, and connect to GitHub using a personal access token.

Please follow these [instructions](./git.md)

### Task 2: Creating a GitHub Repository

In this task, you will create a GitHub repository for your project without initializing the README file.

1. Visit [https://github.com](https://github.com) and log in to your GitHub account.

2. Click on the "New" button to create a new repository.

3. Enter a repository name and, if desired, provide a description.

4. Make sure to **uncheck** the option "Initialize this repository with a README."

5. Optionally, choose a license and add a `.gitignore` file if needed.

6. Click the "Create repository" button.
7.  follow the guidelines:
```sh
echo "# Readings" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/???/???
git push -u origin main
```

### Task 3: Edit the README.md File

In this task, you will edit the `README.md` file and push your changes to GitHub

1. Open the `README.md` file 

- Add a Header 1 (`#`) with the title of your project.
- Add a Header 2 (`##`) with a subheading.
- Create an unordered list using asterisks or hyphens (`*` or `-`) to list some items.

Example:

```markdown
# My Project

## Subheading

* Item 1
* Item 2
* Item 3

## Subheading

* Item 1
* Item 2
* Item 3
```

2. Push your changes to GitHub
```sh
git add .
git commit -m "message here"
git push -u origin main
```


