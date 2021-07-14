# Git Setup

The Rover team has a Git Organisation which you must request access to via the current Software Leader/Architect. You can use a Student or Personal Git account.

## Setting Up SSH

This tutorial is more indepth and will be kept up to date more [here](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

Login to Git and navigate to your [key list](https://github.com/settings/keys).

If you are using WSL2 Ubuntu 18.04
```
sudo vim /etc/wsl.conf
```
Copy and paste the following into the editor, Save and Exit.

```
[automount]
options = "metadata"
```

Close all WSL terminals and run in powershell
```
wsl --shutdown
```

In ubuntu 18.04

```
ssh-keygen -t ed25519 -C "s1234567@student.rmit.edu.au"
```

```
git config --global user.name "s1234567"
git config --global user.email "s1234567@student.rmit.edu.au"
```


Copy and Paste the result from this command into a `New SSH Key` on Github.
```
cat ~/.ssh/id_ed25519.pub
```

In your ROVER_WS. [Set this up in Environment](ROS Setup.md)

Clone this repo to test.
```
git clone git@github.com:RMIT-Rover/rmit_rover_description.git
```

