Day 7 Task: Understanding package manager and systemctl

What is a package manager in Linux?
In simpler words, a package manager is a tool that allows users to install, remove, upgrade, configure and manage software packages on an operating system. The package manager can be a graphical application like a software center or a command line tool like apt-get or pacman.

You’ll often find me using the term ‘package’ in tutorials and articles, To understand package manager, you must understand what a package is.

What is a package?
A package is usually referred to an application but it could be a GUI application, command line tool or a software library (required by other software programs). A package is essentially an archive file containing the binary executable, configuration file and sometimes information about the dependencies.

Different kinds of package managers
Package Managers differ based on packaging system but same packaging system may have more than one package manager.

For example, RPM has Yum and DNF package managers. For DEB, you have apt-get, aptitude command line based package managers.

Tasks
You have to install docker and jenkins in your system from your terminal using package managers

Write a small blog or article to install these tools using package managers on Ubuntu and CentOS

systemctl and systemd
systemctl is used to examine and control the state of “systemd” system and service manager. systemd is system and service manager for Unix like operating systems(most of the distributions, not all).

Tasks
check the status of docker service in your system (make sure you completed above tasks, else docker won't be installed)

stop the service jenkins and post before and after screenshots

read about the commands systemctl vs service

eg. systemctl status docker vs service docker status