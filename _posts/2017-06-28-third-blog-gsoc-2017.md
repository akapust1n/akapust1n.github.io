This is my report for the last month.

This month was quite difficult, I took exams at the university, so I did not do as much as I wanted.
For this month I did:
 - Collecting system information
   At now a can to collect information about cpu, video card, qt version, krita version, compiler version and information about system.
   ([my branch](https://github.com/KDE/krita/tree/akapustin/T6102-telemetry))
 - Create server, which can recieve info from clients, write info to database and give data to fronted.
   There is some troubles with database. Server can work with PostgreSQl, but KDE doesn't want to use PostgreSQL. I will rewrite it to MongoDB.
   ([my repository](https://cgit.kde.org/websites/telemetry-krita-org.git/))
 - Create simple frontend for tree-view of information
    Now the frontend is written on Nodejs. KDE doesnt want to use Nodejs too :(. I will rewrite it to Python.

Plans:
 - Create tests and setup  continuous integration for backend servers.
 - Make a system for collecting information about tools


