[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12769902&assignment_repo_type=AssignmentRepo)
# Template for project 1 retake

This repository is your group's place to store all files for the implementation phase of Project 1. The Analysis and Design artefacts are still stored on OneDrive, which you have worked with the past weeks.

You are free to re-structure this repository to your liking, but make sure that you have a system and it's not chaotic!

If you are unsure, just use the template as given. Your repository is structured the following way:

`./website`: html/php files

`./website/images`: images

`./website/styles`: css files

You can create more folders if you need them! Separate images from music files, find a good place to store documentation that you may need, and so on!

## Start the application

> :warning: Docker should be installed, if not follow the instructions from [https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/)

1. Copy (do not only rename) the `.env-example` and rename the file to `.env`, make sure the leading 'dot' stays there.
    - Files starting with a `.` are automatically hidden on Linux/MacOS, make sure to show hidden files 
2. Only Linux and MacOS users, change the values of `UID` and `GID` in the `.env` file according to your system
     - To get the correct values, in the terminal type the following commands for `UID` and `GID` respecively:
        - `id -u`
        - `id -g`
3. Open a terminal at the location where you cloned this repository
    - Open a terminal and use `cd` to get to the correct location
    - Or right click in finder/explorer and `Open in terminal`
4. To start the application type the following command:
    - `docker compose up -d`
    - It may take a while on the first start :)
5. Open your favorite browser and go to [http://127.0.0.1/](http://127.0.0.1/) and it should show a page indicating that everything is working.
6. To stop the docker containters run the following command:
    - `docker compose stop`
7. Now it is also possible to start/stop the container from Docker Desktop