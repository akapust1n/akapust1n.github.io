Hello, this is the report for the second phase of the GSOC.

The last month was not easy. Some things had to be re-written because they were not very well written. For example, I wrote a system of "sensors", the logic of which was laid in the destructors of objects. This is a non-obvious logic of work, it had to be rewritten.

The provider for telemetry collection had to be placed in a separate top-level library.Now for telemetry there is a plugin and a separate library. I made a system for collecting information about tools. I also made a system for collecting information about image properties. How does it work? If the user saves the image, information about the image is recorded in the special data structure. If the user again saves the same image, then the information about this image is updated. However, if the user restarts the program, information about the images will be recorded again. A system for collecting information about the asserts was made. How does it work?The program "drops" -> the user restarts the program-> information about the last "fall" is sent to the server.

It was also started rewriting the frontend to the python and collecting information about the tools was implemented by the backend.
