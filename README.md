





Technology Template
MongoDB & Python on Ubuntu 11.10

Student: Naidin Mihaela Loredana





MongoDB on Ubuntu 11.10, 32bit

To install MongoDB, run the following command:
sudo apt-get update; sudo apt-get install mongodb
Then, download the corresponding version(32bit):
wget http://www.mongodb.org/dr/fastdl.mongodb.org/linux/mongodb-linux-i686-2.2.1.tgz/download
Extract the archive:
tar xfz mongodb-linux-i686-2.2.1.tgz
Create a new folder for mongodb:
sudo mkdir /usr/local/mongodb
And add the bin directory to my $PATH:
sudo cp -r mongodb-linux-i686-2.2.1/bin /usr/local/mongodb/
export PATH=$PATH:/usr/local/mongodb/bin
Now, you can start the MongoDB Shell, by typing mongo in a terminal.

 
Setting up a Python Environment withMongoDB

	In order to be able to connect to MongoDB with Python, you need to install the Py-Mongo driver package.

	The best practice is to create what is known as a “virtual environment” in which to install your packages.
The tool to create a “virtual environment” is called virtualenv.
To install it on ubuntu simply run:
sudo apt-get install python-virtualenv
Now, to create the first virtual Python environment, run:
virtualenv –no-site-packages myenv.

To install PyMongo run:
sudo bin/easy_install pymongo
in myenv directory


To check that the installation worked, run:
python import pymongo
while you are still in mydev directory.
or python help(pymongo) to see more information about it.

	Now the PyMongo driver is installed correctly and ready to connect to MongoDB and start
issuing queries!

	To launch the mongodb GUI, python-run the file  app.py and enter the port number 27017 on localhost to list all databases and collections.
