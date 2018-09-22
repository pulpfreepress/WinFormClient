# WinFormClient
A C# Windows Forms client that can send and receive commands to/from a connected server.

This application is meant to be used in conjunction with the WinFormServer which is located in another repository.

This code is an educational framework that demonstrates fundamental concepts in multi-threaded client-server application programming. It demonstrates the following concepts:

- How to parse IP address string using IPAddress.TryParse()
- How to parse Port number strings using Int32.TryParse()
- How to both send and receive commands to and from a server
- How to access UI components running on the main thread from a different thread

Notes: Error handling is not robustly implemented, but sufficiently so. In some cases, exceptions are logged to the large status text box. 

Commands between client and server can be expanded by adding applicaple case statements to the switch statement located in the ProcessClientTransactions() method. A corresponding change must also be made in the WinFormClient application's ProcessClientRequests() method.
