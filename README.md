# ftp
<pre>
The system is a multi-client server structure, based on UDP protocol stop-and-wait process, file transmission program. 
Moreover, checksum method and retransmit mechanism for error control are implemented.

Notice: The program must be executed by superuser privileges.
        To make sure the correctness of processing, specify NIC is needed.

client: 1. Usage => ./myftpClient &ltport #&gt &ltfile name&gt 
        2. Connect to server.  
server: 1. Usage => ./myftpServer &ltport #&gt &ltfile name&gt  
        2. Use multi-thread to handle requests from clients.  
        3. 10% probability to make wrong checksum in order to test the reaction of client and the retransmission of server.
</pre>