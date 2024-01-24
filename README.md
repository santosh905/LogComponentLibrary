# LogComponentLibrary
LOGGER LIBRARY - Client/application make use of  logger library to log messages to a sink
Message -
      - has content which is of type string has a level associated with it
    - is directed to a destination (sink)
    - has namespace associated with it to identify the part of application that sent the message
  Sink-
    - This is the destination for a message (eg text file, database, console, etc) Sink is tied to one or more message level
Feature of Logger Library - 
  - Requires configuration during sink setup
  - Accepts messages from client(s)
  - Routes messages to appropriate sink based on the level
   - Supports following message level in the order of priority: FATAL, ERROR, WARN, INFO, DEBUG 

Sending messages-
• Sink need not be mentioned while sending a message to the logger library.
• Use can specify message content and level 

Logger configuration- 

•Library accepts one or more configuration for an application as below
1. Filepath of logfile
2. database connection(as of now it supports SQL Server)

Silient Feature of the Library.
1. Logs message asyncronously
2. Threadsafe
3. Code is covered with unit testing
4. LogTarget is changed dynamicaly based on the loglevel selected by user while loging and it can be configured based on the user's requirment using configuration file.
