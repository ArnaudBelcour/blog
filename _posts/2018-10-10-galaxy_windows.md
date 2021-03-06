---
layout: post
date: '2018-10-10'
title: "A Galaxy at the Windows"
---

Using Galaxy on Windows with the Windows Subsystem for Linux.

## Windows Subsystem for Linux (WSL)

WSL is a compatibility layer developed by Microsoft and Canonical. It runs only on Windows 10 64-bits (you can see the installation process [here](https://msdn.microsoft.com/commandline/wsl/about)).

## To Galaxy and beyond

Clone the Galaxy repository using WSL and use the command for the Linux system installation ([here](https://galaxyproject.org/admin/get-galaxy/#get-started)).
You have to clone the Galaxy repository inside the WSL environment if not, perl and python dependencies will not be installed.

Now, a Galaxy local server is running.

In Windows, files are stored in ‘C:\Users\<USERNAME>\AppData\Local\lxss\home\Galaxy’. To have administrator right in Galaxy, open the ‘config/galaxy.ini.sample’ file with vim (from WSL) and modify it. Do not use an editor from Windows, it will break Galaxy.

And then you will have a Galaxy at your window!

<img src="{{site.baseurl}}/images/galaxy_windows.png" alt="gitlab_icon">
