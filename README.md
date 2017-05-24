# file-transfer
  A simple file transfer project to practice socket and Boost filesystem programming. This is not a serious program to be used, just something I made to send files between my computers. This program has only been tested on Linux filesystems.

  The project consists of a server program and client program. The programs must be installed on computers on the same network to function.
  
  The server program displays the computer's network interfaces, and lets the user choose an interface to use. A socket is opened on the selected interface, and the server program waits for an incoming connection.

  The client program asks for the server's interface number and port number, and establishes a connection. The client program then waits for commands from the server program.
  
  The server program is able to display the current working directory, and any files inside. The user may send any files in the current working directory, or change directories using relative pathing. If the user attempts to send a file that has an identical name on the client's side, the client will be asked to continue. Currently, sending a file that exists on the client side will append the contents of the server's file onto the client's file. The client's file will NOT be replaced.
