Hello. Recently, within the framework of my project, the following was done:
 - Collection and sending of basic information about the user's system 
 - Accept and write it to the database on the server
 - Frontend for visualization of this information(prototype)

### How do I store this information?
It was decided that using sql is unreasonable because of the large amount of data.
Therefore, the method of storing the Postgresql json data was chosen, which makes it possible to flexibly approach the filling of the database and handle large amounts of data.

### How does the frontend take information from the database?
Once per hour starts a process(goroutine) that aggregates information from the main database into an additional one. From this additional database takes information front-end.

### What to do next?
So far I only collect basic system information. It is necessary to expand the sources of information collection.
[Repository with my servers](https://github.com/akapust1n/kritaServers)
