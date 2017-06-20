**This project is deprecated. See [Install MOLGENIS with Docker](https://github.com/molgenis/docker/) to install the latest MOLGENIS version.**

# molgenis-cargo

This maven project allows you to download a released molgenis war file from maven central, download apache tomcat, 
and run molgenis locally in tomcat.
You need java, maven, and a postgresql database with a user who's been granted full privileges on the database.

For a clean run:

    mvn clean resources:resources org.codehaus.cargo:cargo-maven2-plugin:run
 
This will remove everything, recreate the database and molgenis properties file and start molgenis.

To restart a stopped instance, just type

    mvn org.codehaus.cargo:cargo-maven2-plugin:run
