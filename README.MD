# Mac Ansible setup script

Sets up a new mac with all tools and programs for development

## Prerequisites

Install the necessary components using [setup-init.sh]("https://gist.github.com/Kelley12/b974736c98713d5ff40a63b6c59d129f", "git-setup.sh") script file

[Add the SSH key to your GitHub account]("https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/", "Add SSH Key to GitHub")

## Execution

    ansible-playbook dev-setup.yml  -i environment/localhost --ask-sudo-pass

To run just a subset of tasks

    ansible-playbook dev-setup.yml  -i environment/localhost --ask-sudo-pass --tags "sublime,bash_alias"

## Other Info

 To add/change the bash alias, edit the /roles/dev-common/files/bash_alias file
