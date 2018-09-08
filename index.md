[TOC]

# Install manually
Navigate to the official web page: https://www.mongodb.com

Then click on [Get MongoDB] button.

On the opened page, choose [Community server] tab.

Then click [Download] button.

Install download file (*.msi).

To make using DB a bit simpler, choose short path for the installation:

`D:/mongodb/data`


#Configuring
## DB path
Navigate to the installation directory then move to \bin folder.

To set db and log file location Run a command:

```
mongod --dbpath D:/mongodb/data/db --logpath d:\mongodb\log\mongodb.log --logappend --install
```

#Run service
## Using Terminal
To run mongoDB service manually run a command:

`mongod --dbpath D:\mongodb\data\db`

## Using \*.bat file
create a file mongodb run `service.bat`

Enter next text:
```
cd /d C:\Program Files\MongoDB\Server\4.0\bin
mongod --dbpath D:\mongodb\data\db
pause
```
Run the file when there is a need to start mongodb service.


#Run service
If mongo command is not recognized by Windows, run a command with a full path:

`"C:\Program Files\MongoDB\Server\4.0\bin\mongo.exe"`
