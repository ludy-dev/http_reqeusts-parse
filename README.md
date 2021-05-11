HTTP Reqeusts message parse with pcre
=====================================

The http request message consists of an http header, denoted by a carriage return '\r\n' [0x0d0a] to indicate the end of the line.
Equipment in some IT systems, including equipment for information security, represents carriage returns as escape sequences. 

Thus, workers see Raw-data represented by \r\n at the end of the header line.

<pre>
<code>
 GET / HTTP/1.1\r\nHost:www...\r\n ...
</code>
</pre>

It is necessary to separate some header fields from this http request message during work, I wrote the pcre using this carriage return as below.

<pre>
<code>
 123
</code>
</pre>


