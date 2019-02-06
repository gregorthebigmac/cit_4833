# Answers

1. How many packets are in this trace file?  
    **A.** 20
2. What IP hosts are making a TCP connection in frames 1, 2, and 3?  
    **A.** 192.168.1.108 and 50.18.228.205
3. What kind of HTTP command is sent in frame 4?  
    **A.** To me, this appears to be a cookie request. I think it's looking for a cached user account.  
    **notes:** vindico|audience|issued|identity (without the '|' chars) was found in the packet.
                looks like a cookie request from a website. I looked up the company, and it turns
                out they're some medical education company. Probably looking for a previously used
                user account.
4. What is the length of the largest frame in this trace file?  
    **A.** Two packets tied for largest:
        <pre><code>Frame 12: 1428
        Frame 15: 1428</code></pre>
5. What are the different kinds of protocols seen in the Protocol column?  
    **A.** HTTP, TCP
6. What responses are sent by the HTTP server?  
    **A.** It looks like *all* of the responses from the HTTP server are
        <pre><code>HTTP/1.1 302 Found</code></pre>
        I found 5 of these responses in frames 6, 8, 10, 13, 16
7. Is there any IPv6 traffic in this trace file?  
    **A.** I wasn't able to find any.