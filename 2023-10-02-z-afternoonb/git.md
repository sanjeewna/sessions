# Git/GitHub

### installation

You can easily install `Git` in Windows by using the [installer].

Once you've downloaded one of the "Git for Windows Setup" distributions (either 32-bit or more likely 64-bit) you can launch the installer and accept all the defaults.


### Configuring git

Once you have installed git, configure the information that gets logged for each
of your commits by updating the default (global) credentials that git uses. (You could overwrite these credentials temporarily per local repo. While that shouldn't be necessary, it is helpful to know that it is an option.) You will also want to set the default branch to `main`.

In your terminal, run

```shell
git config --global user.name "Your Name"
git config --global user.email "Your Email"
git config --global init.defaultBranch main
```

Check that your name and email have been set up correctly by using the following commands:

```shell
git config user.name
git config user.email
```

You should see your name and email address returned. Repeat this step if there
are any errors.

### Configuring GitHub

GitHub provides a mechanism to share code with other
developers. Because of the nature of code, there needs to be a way to authenticate to make sure that someone is authorized to fetch or contribute new
code.

Thankfully, git handles this authentication flow automatically. But for GitHub, you can't use your GitHub account password. Instead, you can use a Personal Access Token (PAT) to authenticate to Github. This way you don't have to use the token with every command that requires authentication.

> Follow the steps in tutorial on [how to use GitHub Personal Access Token (PAT) in VSCode](https://linuxpip.org/use-github-personal-access-token-in-vscode/?utm_content=cmp-true)


[installer]:https://git-scm.com/download/win