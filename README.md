TT_app.py
=========
Setup mongoDB and use a python GUI to output it's records.
Purpose 
=======
The purpose of this TT is to guide you through all the necessary steps that are 
required before you can use a python-based app to view records of mongodb.
Requirements
============
A PC with internet access that is running Ubuntu 11.10.
HowTo
=====
1. install mongoDB "sudo apt-get update; sudo apt-get install mongodb"
2. Download the corresponding version (32/64bit) "wget http://www.mongodb.org/dr/fastdl.mongodb.org/linux/mongodb-linux-i686-2.2.1.tgz/download" and extract it.
3. Create a new folder "sudo mkdir /usr/local/mongodb" and add the bin directory to my $PATH: "sudo cp -r mongodb-linux-i686-2.2.1/bin /usr/local/mongodb/ ; 
export PATH=$PATH:/usr/local/mongodb/bin"
4. Start the MongoDB Shell, by typing "mongo" in a terminal
5. To install Py-mongo, first install virtualenv "sudo apt-get install python-virtualenv" and create the first virtual Python environment "virtualenv –no-site-packages myenv"
6. Install Pymongo "sudo bin/easy_install pymongo" (in mydev directory)
7. Check if installation worked "python import pymongo"
8. Run app.py in your favourite software development environment

Resources used
==============
1. Python -  http://python.org/
2. Eclipse - http://www.eclipse.org/
3. MongoDB - http://www.mongodb.org/

Questions?
==========
E-mail: mihaelaloredan4@gmail.com
