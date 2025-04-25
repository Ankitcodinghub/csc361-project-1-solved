# csc361-project-1-solved



**<span style='color:red'>TO GET THIS SOLUTION VISIT:</span>** https://www.ankitcodinghub.com/product/csc361-there-are-two-tutorials-t2-and-t3-and-two-lab-sessions-l2-and-l3-associated-with-this-assignment-solved/

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;128326&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSC361 Project 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">
            
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
            5/5 - (2 votes)    </div>
    </div>
&nbsp;

There are two tutorials (T2 and T3) and two lab sessions (L2 and L3) associated with this assignment.SWS requirements:

SWS only supports the “GET /filename HTTP/1.0” command, and “Connection: keep-alive” and “Connection: close” request and response header when supporting persistent HTTP connection. The request header is terminated by an empty line known as “ ”, where “ ” indicates a carriage return and “ ” a (new) line feed.

If unsupported commands are received or in unrecognized format, SWS will respond “HTTP/1.0 400 Bad Request”. If the file indicated by filename is inaccessible, SWS will return “HTTP/1.0 404 Not Found”. Such responses will be followed by the response header if any, an empty line, indicating the end of the response.

For successful requests, SWS will respond “HTTP/1.0 200 OK”, followed by the response header if any, an empty line indicating the end of the response header, and the content of the file.

How to run SWS:

On H2 in PicoNet, “python3 sws.py ip_address port_number”, where ip_address and port_number indicate where SWS binds its socket for incoming requests.

1

On H1 in PicoNet, “nc sws_ip_address sws_port_number” to connect to SWS, and type “GET /sws.py HTTP/1.0” followed by “Connection: keep-alive” and an empty line to request the file sws.py from SWS (in this case, SWS shall keep the connection alive after sending back sws.py following an empty line after

“Connection: keep-alive”, and wait for the next request from the same client through the same TCP connection, until the connection times out, i.e., “Connection: close”). If the client does not include “Connection: keep-alive” or does include “Connection: close” in its request, SWS will close the connection after serving the request.

How to test SWS:

Capture and analyze the interaction between SWS and its clients (nc, wget or even a regular web browser) with tcpdump and Wireshark. Your code will be evaluated in PicoLab as you have in ECS360.

What to submit:

sws.py source file, and the tcpdump files on R, showing the interaction between SWS and its clients, in both persistent (sws-persistent.cap) and non-persistent (sws-non-persistent.cap) connections. Please also copy and paste the content of sws.py and tcpdump -r the capture file to the text input box on brightspace.

When:

2

Appendix: A simple design for your reference

3
