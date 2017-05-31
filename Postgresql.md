Postgres and Postico Install

Postgres Overview

Postgres is a SQL database. This guide merely shows you how to install the software needed to run Postgres. Actual lectures on using Postgres will follow.

Prerequisites

You have previously installed Homebrew, the package manager for Mac OS. You have recently updated Homebrew. Open a terminal Type brew update Press enter key Installation

Open a terminal Type brew install postgres (and type enter key) Starting/Stopping Postgres (Option 1 of 2)

If you have installed Postgres with Homebrew, you can use the built-in Brew Services commands to start/stop the server as below:

Stop the server: brew services stop postgresql Start the server: brew services start postgresql Starting/Stopping Postgres (Option 2 of 2)

In your terminal, type postgres -D /usr/local/var/postgres to start Postgres using the specified file location as a data directory To stop Postgres, press the control and C keys at the same time Create an Environment Variable Postgres (optional)

You might find it inconvenient to start postgres by typing in all of that stuff. You can make your life easier, by setting a PGDATA environment variable.

Open a terminal Type ~ and press enter key to get to your user's directory Open and/or create a file named .bash_profile Add the following line to the file: export PGDATA="/usr/local/var/postgres" Save the file. Close the terminal window. Open a new terminal window (to see the changes take effect). Type postgres and press enter key to start your database. Postico (Database Client GUI app) Overview

At this point we will have a Postgres server program running on our local computer. We're now going to install a graphical client so we can have an easy way to interact with our new server software.

Installation

Go to: <https://eggerapps.at/postico/> Download Unzip and move to your Applications folder Open (double-click Postico icon) First thing we need to do is establish a connection to our server. It's running locally.

Postico

Localhost

By default, Postgres creates a database called whatever your username is. Here "krisszafranski" is Kris Szafranski's username.

Known Issues

IMPORTANT: Only complete the following steps if you get an error when you try to connect stating this database does not exist.

To manually create your database

Open a Terminal Type createdb $USER Now back in Postico you should be able to connect to the host: localhost with a database called your username.
