Advanced Nagios Plugins Collection
==================================

I've been developing this Nagios Plugin Collection since around 2006. The basic Nagios plugins collection is a great base to start from, while this extends Nagios monitoring capabilities further especially in to the application layer. I highly recommended that all Nagios users consider becoming familiar with these tools.

These programs can also be run standalone on the command line or used in scripts as well.

Despite the recent timestamps this is actually an aggregation of various sources where I've previously released my code over the years such as Nagios Exchange and Monitoring Exchange. I finally got round to re-releasing them come under one place for better maintainance and support.

### Setup ###
The first thing you need to do is to get my library submodule since I share code between this and other things that I have written over the years.

Enter the directory and run git submodule init and git submodule update to fetch my library repo:

```
cd nagios-plugins
```
```
git submodule init
```
```
git submodule update
```
This will pull in my git library repo which several of these plugins require to give very robust validation functions, utility functions, logging levels and debugging etc

You're now ready to use these programs.

### Other Dependencies ###

Most plugins will now run as is with minimal dependencies. Some plugins, notably some of those under the legacy directory such as those that check 3ware/LSI raid controllers, SVN, VNC etc require external binaries to work, but the plugins will tell you if they are missing. Please see the respective vendor websites for 3ware, LSI etc to fetch those binaries and then re-run the plugins where needed.

### Usage ###

All plugins come with --help to list all these options and are named fairly intuitively as well as having a description in the header at the top of each file.

Usage examples will be added here soon