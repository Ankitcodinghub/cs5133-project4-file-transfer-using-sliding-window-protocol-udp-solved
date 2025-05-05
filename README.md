# cs5133-project4-file-transfer-using-sliding-window-protocol-udp-solved
**TO GET THIS SOLUTION VISIT:** [CS5133 Project4-File Transfer using Sliding Window Protocol UDP Solved](https://www.ankitcodinghub.com/product/cs5133-project4-file-transfer-using-sliding-window-protocol-udp-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;72309&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS5133 Project4-File Transfer using Sliding Window Protocol UDP Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
The objective of this programming project is to learn UDP reliable client-server interaction using UDP socket interface in C programming language. After completing the project, you will have a basic understanding of the steps required to add reliability features in UDP applications for developing a networking application.

<ol start="2">
<li><strong>Project Specification: </strong>
<ul>
<li><strong>Overall System Behavior: </strong></li>
</ul>
</li>
</ol>
You are required to implement a reliable simple file transfer protocol which uses the Selective repeat sliding window protocol for data and flow control. For detail about the Selective repeat sliding window protocol, please refer to your textbook (<em>Andrew S. Tanenbaum</em>, “Computer Networks”, Prentice Hall, Fourth edition., Page 211). Selective repeat is the basic mechanisms used in reliable window-based process to process communication protocol. The Selective repeat window protocol contains a <em>sender window.</em> There is also a <em>receiver window</em> that allows the receiver to buffer packets received in any order. The essence of the selective repeat protocols is that at any instant of time, the sender maintains a set of sequence numbers corresponding to frames it is permitted to send. These frames are said to fall within the sending window. Similarly, the receiver also maintains a receiving window corresponding to the set of frames it is permitted to accept. The receiver can explicitly request retransmission of a “<strong>missing</strong>” packet from the receiver by sending a <em>negative acknowledgement. </em>The following figure shows high-level overall system requirements.

<ul>
<li><strong>Sender Behavior [Server]: </strong>
<ul>
<li>At startup, the sender takes two arguments that specify the port number that it is listening to and the window size. You have to use (<em>5000</em>+<em>last 4 digits</em> of your student-id number) to avoid requesting same port by multiple students. The second parameter, window size, of the sender must be &gt; 1.</li>
<li>After successful startup, the sender program will wait for a UDP client interaction for <strong>user authentication</strong>. Server has <em>txt</em> file which contains username and password separated by a blank space. If authentication is successful, then sender will wait for a file transfer using UDP.</li>
<li>After receiving a file name from the client, sender process will verify the existence and read permission of the file. If the file doesn’t exist or permission denied, then the sender will transmit appropriate warning message back to client and wait for a new valid file name.</li>
<li>If the file exists and read permission granted, then sender will send the window size (sender and receiver has same window size) and start transmitting data using UDP packet to client. You may use <strong>128/256 bytes of payload</strong> per packet.</li>
<li>Your sender program should handle this packet transfer using Selective-Repeat Sliding Window Protocol discussed earlier.</li>
<li>The protocol identifies the DATA segments by using <strong>sequence numbers</strong>. The sequence number of the first segment must be 0. It is incremented by one for each new segment. The receiver must acknowledge the delivered segments by sending an ACK segment.</li>
<li>Along with each data packet, you need to deploy a <strong>timer</strong> to keep track of delayed or lost ACK/NACK packets from the receiver.</li>
<li>As the sender program receives ACK from the receiver, it needs to randomly <strong>drop 10%</strong> of the ACK to simulate ACK lost from the receiver (generate random numbers to handle this requirement). You need to retransmit based on the Selective Repeat protocol before sliding the sender’s window. The flow of data is unidirectional, meaning that the sender only sends DATA segments and the receiver only sends ACK segments.</li>
<li>Finally, when the data transmission is complete, your sender program will go back and wait for another UDP client communication for next user authentication and file transfer.</li>
</ul>
</li>
</ul>
&nbsp;

<ul>
<li><strong>Sender Output: </strong>
<ul>
<li>You need to print <em>SEQ number</em> and <em>type of operation</em> (transmission/retransmission) message after sending the data packet so that we can see your processes are working correctly (or not!).</li>
<li>After successful transmission/retransmission of packets, when the file transfer is complete, your sender program should print the following<strong> statistical report</strong> about the whole transmission.
<ul>
<li>Receiver IP and Port Number</li>
<li>Name and Size of the file that was transferred o File Creation Date &amp; Time</li>
<li>Number of Data Packets Transmitted o Number of Packets Re-transmitted o Number of Acknowledgement Received</li>
<li>Number of Negative Acknowledgement Received with Sequence Number</li>
</ul>
</li>
</ul>
</li>
</ul>
&nbsp;

<ul>
<li><strong>Receiver Behavior [Client]: </strong>
<ul>
<li>Your client program takes four arguments from user during startup that specifies the IP address and port number of the sender, input file name that receiver wants to copy from the sender and the output file name which will be used for creating the new file at receiver side.</li>
<li>After a successful startup, your receiver program will print a welcome message and ask the user to input username and password for login into the sender program (server).</li>
<li>These data will be sent to the receiver program using UDP for the user authentication. Then, your sender, after receiving the username and password from the receiver, will verify the received pair of username and password against the pairs in userList.txt file. If the result is positive, the server will send a success message to the receiver along with the window size (sender and receiver has same window size). If the result is negative, the server will send an error message to the sender and wait for the new pair.</li>
<li>After successful authentication, your receiver program will ask the user whether to start the file transfer or not. With a positive feedback, the input file name will be sent to the sender program to verify the existence and access permission.</li>
<li>If file doesn’t exist or permission denied, the sender program will inform the receiver. You need to print the message and prompt the user for a new valid file name. If the file exists and read permission granted, then receiver will create an output file and start copying the incoming data into the file. <em>Note, UDP packets may come unordered. You need to keep track of it using the sequence number. </em></li>
<li>Your receiver program should handle this ACK/NACK packet transfer using Selective-Repeat Sliding Window Protocol discussed in the class.</li>
<li>As the receiver program receives data packets from the sender, you need to randomly <strong>drop 10%</strong> of the data packets to simulate the data lost (generate random numbers to handle this requirement). You need to send NACK packet based on the Selective Repeat protocol before sliding receiver window for new set of packet(s).</li>
<li>When the file is completely received, your receiver will go back and ask the user whether they wants to send any more file or not.</li>
</ul>
</li>
</ul>
&nbsp;

<ul>
<li><strong>Receiver Output: </strong>
<ul>
<li>You need to print informative message after receiving a data packet and sending an ACK/NACK packets so that we can see your processes are working correctly (or not!).</li>
<li>After successful file receive, your receiver program should print the following<strong> statistical report</strong> about the whole transmission.
<ul>
<li>Name and Size of the file that was received</li>
<li>File Creation Date &amp; Time o Number of Data Packets received o Number of Acknowledgement Sent o Number of Negative Acknowledgement Sent</li>
</ul>
</li>
</ul>
</li>
</ul>
&nbsp;

<ul>
<li><strong>Input Format: </strong></li>
</ul>
Sender and receiver must be command-line tools that allow transmitting one binary file and supporting the following parameters:

<strong>&nbsp;sender</strong> &lt;port_number&gt; &lt;window_size&gt;

<strong>&nbsp;</strong>

<strong>&nbsp;receiver</strong> &lt;sender_ip&gt; &lt;sender_port&gt; &lt;input_file&gt; &lt;output_file&gt;

&nbsp;

<ol start="3">
<li><strong>Programming Notes: </strong></li>
</ol>
<strong>&nbsp;</strong>

You have to use UDP sockets for implementing both sender and receiver programs. You should program each process to print an informative statement whenever it takes an action (e.g., sends or receives a message, detects termination of input, etc), so that you can see that your processes are working correctly or not. One should be able to determine from this output if your processes are working correctly. You should hand in screen shots (or file content, if your process is writing to a file) of these informative messages.

Make sure, your Sender (server) allows the user to specify the listening port number and window size during startup. You have to close every socket that you use in your program. If you abort your program, the socket may still hang around and the next time you try and bind a new socket to the port ID you previously used (but never closed), you may get an error. Also, please be aware that port ID’s, when bound to sockets, are system-wide values and thus other students may be using the port number you are trying to use though it’s prohibited. . If you need to kill a process after you have started it, you can use the LINUX <em>kill</em> command. Use the LINUX <em>ps</em> command to find the process id of your server.

Any clarifications and revisions to the project will be posted on the course web page on Canvas. Students are encouraged to start this project early and use the project discussion group on Canvas for any general question so that everyone can benefit from the replies.

<strong>File names:</strong>

File names for this project are as follows:

Client: <em>lastNameSelectiveRepeatReceiver.c </em>

Server:<em> lastNameSelectiveRepeatSender.c </em>
