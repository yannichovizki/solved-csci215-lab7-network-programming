Download Link: https://assignmentchef.com/product/solved-csci215-lab7-network-programming
<br>
Question 1: Value sharing via UDP

Write a program where the initial parent process creates N child processes, then creates a UDP socket and binds it to port 5678, and after that waits for their messages. Each child generates a random value random_val, sends it to the parent address and displays it before exiting. The random value is generated thus:

random_val = rand ()%10;

The parent process sums up all the values it has received, then displays the result, and finally waits for its children to terminate.

Question 2: File exchange via TCP

Write a program that sends the contents of a file from one host to a remote host by means of a TCP connection.

The sender program is run with:

$ sendfile &lt;addr&gt; &lt;port&gt; &lt;filename&gt; where addr is the address at which the receiver waits for connection requests port is the port number on which the receiver waits for connection requests filename is the name of the file to send

When it obtains its connection with the receiving program, the sender first sends a first packet with the name of the file. All the following packets contain the contents of the file.

The receiver program is run with:

$ recvfile &lt;port&gt; where port is the port number on which the receiver waits for connection requests

The receiving program stores the copied files in its execution directory.


