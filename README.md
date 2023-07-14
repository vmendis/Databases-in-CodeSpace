# Databases-in-CodeSpace
Run databases and the GUI access to it in a GitHub CodeSpace.

I had this urge (itch) to run a database (initially MySQL) and the GUI access to it, all running in a GitHub CodeSpace.
This repo is the result of it.

While I was experimenting ways to accomplish my objectives, I came across this site which contains the necessary docker-compose files
https://www.codeproject.com/Tips/5336563/Run-Database-and-GUI-Clients-in-Docker


Quick introduction to docker compose: https://github.com/docker/compose

I use 'gh ssh' from a Mac to connect to my GitHub CodeSpaces for the conveniences. You can run the commands from the CodeSpace terminal available in your browser as well.

Disclaimer: This is only a prrof-of-concept work. Use the solution for learning and testing. Do not store real life data, unencrypted passwords, production data etc.

Working Solutions:

MySQL + phpMyAdmin
   $ cd MySQL-PhpMyAdmin
   $ docker-compose up
   PhpMyAdmin is available on Port 5013. Simply click Port 5013 in the "Local Address" column in "PORTS" tab. A new tab will be opened.
       Server = MySQL
       Username = citizix_user
       Password = An0thrS3crt

        NOTE: The credentials are from the original author. User citizix_user does not have any privilages to create databases. Please create your own user with the necessary privilages to administer databases.
    $ docker-compose down


