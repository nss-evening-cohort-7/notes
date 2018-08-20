# Setup

### [Visual Studio Community Edition](https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Community&rel=1)
- At the beginning there will be a lot of boxes that you can choose to install.  We'll show you which ones to pick.

### [SQL Server](https://go.microsoft.com/fwlink/?linkid=853017)
- When installing there will be a prompt for whether you want basic or custom.  we want custom
  - Pay attention to the prompts, we want the default instance, not a named instance, and mixed mode authentication

### [SQL Server Management Studio](https://go.microsoft.com/fwlink/?linkid=864329) (SSMS)

### [KDiff3](https://sourceforge.net/projects/kdiff3/files/kdiff3/0.9.98/KDiff3-64bit-Setup_0.9.98-2.exe/download) (git merge tool)
- After installation, use these commands to set KDiff3 as your command line merge tool.
  - `git config --global --add merge.tool kdiff3`
  - `git config --global --add mergetool.kdiff3.path "C:/Program Files/KDiff3/kdiff3.exe"`

### Setting up your SSH key in your VM
Go through this walkthrough to set up git to connect to your github account
- [Generating a new SSH key and adding it to the ssh-agent](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)
- [Adding a new SSH key to your GitHub account](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/)
