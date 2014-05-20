This is a simple playlist application built with Apache Cassandra DataStax Edition 

Building and Running on Unix
-----

1. Install Java 7 JDK.  Validate it with `java -version`   It should be 1.7.  Validate the compiler as well with `javac -version`

2. Install Maven

3. build the project from the classproject directory by typing `mvn install`

4. set up the database

    cd scripts/cql
    cqlsh -f playlist.cql

5. To run it, cd to the target directory

run the main class:

    java -cp 'playlist-1.0-SNAPSHOT.jar:lib/*' StartJetty

6. Visit the application at `http://localhost:8080/playlist`

