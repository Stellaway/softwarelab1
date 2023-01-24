﻿# MongoDB

In this lab, we will work with the MongoDB NoSQL database and the Mongo C# driver.

## Pre-requisites and preparation

Required tools to complete the tasks:

- Windows, Linux, or macOS: All tools are platform-independent, or a platform-independent alternative is available.
- MongoDB Community Server ([download](https://www.mongodb.com/download-center/community))
- Robo 3T ([download](https://robomongo.org/download))
    - Without installing you can run the server with the following command using Docker:
    
          ```cmd
        docker run --name swlab1-mongo -p 27017:27017 -d mongo
        ```
        
- Sample database initialization script: ([mongo.js](https://bmeviauac01.github.io/adatvezerelt/db/mongo.js))
- GitHub account and a git client
- Microsoft Visual Studio 2022 [with the settings here](../VisualStudio.md)
    - When using Linux or macOS, you can use Visual Studio Code, the .NET SDK, and [dotnet CLI](https://docs.microsoft.com/en-us/dotnet/core/tools/).
- [.NET Core **6.0** SDK](https://dotnet.microsoft.com/en-us/download/dotnet/6.0)

    !!! warning ".NET 6.0"
        Mind the version! You need .NET SDK version **6.0** to solve these exercises.

        On Windows it might already be installed along with Visual Studio (see [here](../VisualStudio.md#check-and-install-net-core-sdk) how to check it); if not, use the link above to install (the SDK and _not_ the runtime). You need to install it manually when using Linux or macOS.

Materials for preparing for this laboratory:

- MongoDB database system and the C# driver
    - Check the materials of _Data-driven systems_ including the [seminars](https://bmeviauac01.github.io/datadriven-en/)
- Official Microsoft tutorial for [WebApi using MongoDB](https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-mongo-app?view=aspnetcore-6.0&tabs=visual-studio)
    - We will not be creating a WebApi in this lab, but the Mongo part is the same.

## Initial steps

Keep in mind that you are expected to follow the [submission process](../GitHub.md).

### Create and check out your Git repository

1. Create your git repository using the invitation link in Moodle. Each lab has a different URL; make sure to use the right one!

1. Wait for the repository creation to complete, then check out the repository.

    !!! warning "Password in the labs"
        If you are not asked for credentials to log in to GitHub in university computer laboratories when checking out the repository, the operation may fail. This is likely due to the machine using someone else's GitHub credentials. Delete these credentials first (see [here](../GitHub-credentials.md)), then retry the checkout.

1. Create a new branch with the name `solution` and work on this branch.

1. Open the checked-out folder and type your Neptun code into the `neptun.txt` file. There should be a single line with the 6 characters of your Neptun code and nothing else in this file.

### Create the database

Follow the steps in the [seminar material](https://bmeviauac01.github.io/datadriven-en/seminar/mongodb/#exercise-0-create-database-open-starter-code) to start the database server and initialize the database.
