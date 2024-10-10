# Version Control
Version control is a system that tracks changes to files over time, allowing you to easily manage, revert, or merge different versions of a project. It's essential because it helps prevent data loss, enables collaboration across teams, and ensures that all changes are recorded, making it easy to fix mistakes or understand how a project has evolved.

# Git
Git is a version control system (VCS) is a tool that helps track changes in files, especially when many people are working on a project. It keeps a history of all changes, so if mistakes happen, you can go back to earlier versions. There are [GUI clients](https://git-scm.com/downloads/guis) available, but I *strongly* advise against them, especially if you will be working in the cloud or on an HPC, such as [Grace](https://docs.ycrc.yale.edu/clusters/grace/).

To test if Git is installed on your computer, copy the following into your terminal

```bash
git --version
```

If git is installed, then you will be prompted with the version number (`git version 2.39.1`). If git is not installed, then you will recieve a message saying `command not found`.

## Installation
Git can be installed from the [Git source code management (SCM) website](https://git-scm.com/downloads) and following the instructions for your operating system. If you us MacOS and the [homebrew package manager](https://brew.sh/) then git can be installed via the following command:

```bash
brew install git
```

Git should come pre-installed on MacOS. However, running this command will update to the latest version which is more feature rich.

# GitHub
GitHub is a website that makes it easy to store these changes in the cloud, share them with others, and collaborate on projects. While Git works on your computer and is the software that manages the version control, GitHub is cloud storage for your code and version control history. GitHub, and other git repository hosting platoforms, helps you manage and share projects online, making teamwork more organized and efficient.

Everybody at Yale has access to a [GitHub enterprise](https://resources.github.com/demo/) account. Although everything is hosted on Yale servers, the downside is any repository hosted here can only be private and can not be made publicly avaiable to anybody on the internet. See [Yale GitHub Enterprise and Support](https://yale.service-now.com/it?id=service_offering&sys_id=bc29b84997f88a506f0430671153af28) for more information.

You can log into to Yale GitHub Enterprise using the following steps:

1. Navigate to [https://github.com/](https://github.com/)
2. Click on `“sign in”` in the top right
3. Enter your EMU for the username. This is most likely `firstname-lastname_yale`. For example, mine is `lucas-gloege_yale`.
4. You do not need a password. Instead, click on  `"sign in with your identity provider"`, which directs you to a page to enter your Yale credentials.

In order for repositories to be public facing, you will need to create another account on GitHub.

!!! note "Yale GitHub Enterprise account"
    Yale uses your `@yale.edu` email address to create the enterprise account. You will either need to use a different email to create a person account or unlink your yale email from the Enterprise account. Keep in mind that multiple email addresses can be associated with a single GitHub account, so you have the option to unlink your yale email from GitHub Enterprise in the future.

## Disconnect from GitHub Enterprise
Here are the steps to diconnect your Yale email address from GitHub enterprise, if you choose to do so:

1. Navigate to [https://github.com/](https://gitub.com/)
2. Click on `“sign in”` in the top right
3. Enter your EMU for the username. This is most likely `firstname-lastname_yale`. For example, mine is `lucas-gloege_yale`.
4. You do not need a password. Instead, click on  `"sign in with your identity provider"`, which directs you to a page to enter your Yale credentials.
5. Once logged in, click on the icon in the top right and navigate to `“settings”`
6. On the left, under `“access”`, select `“email”`
7. Click the box next your yale email address that says `“unverify”`. This will disconnect your yale email from the enterprise account.

If you do this, you will still be able to log into GitHub Enterprise at Yale, but your email will be unverified. The benefit of doing this is you can avail the [GitHub Education Benefits](https://education.github.com/discount_requests/application) and your repostories can be publicly avaialble.