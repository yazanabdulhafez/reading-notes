# WRRC and Java

## The HTTP Request Lifecycle

![wrrc](https://miro.medium.com/max/1378/1*4SEvcz6KvyaqOqBpJABTBg.png)

### Step 1: Local Processing

1. the  browser extracts the: "scheme"/protocol, host, optional port number, resource path, and query strings.

2. Browser has the intended hostname for the request, it needs to resolve an IP address,then the browser look through its own cache of recently requested URLs, the operating system’s cache of recent queries, router’s cache, and  DNS cache.

### Step 2: Resolve an IP

1. If the cache lookup fails,  browser fires off a DNS request using User Datagram Protocol (UDP).

2. request will now have to travel many network devices to reach its target DNS server.

3. Once  request arrives at configured DNS server, the server looks for the address associated with the requested hostname.

4. If it finds one, it sends a response.
If an address for the given domain cannot be resolved, the server responds with a failure and your browser returns an error.
If the response makes it back the requesting client now has a target IP.

### Step 3: Establish a TCP Connection

1. One of the key differences between TCP and UDP is that TCP ensures delivery and ordered data transmission.Much of this is done very simply, using what’s known as a sequence number for every byte sent.

2. TCP connections are opened using a three-way handshake. The server must already be "listening" on a port, performing a passive open, after which the client can initiate an active open, and the handshake works as follows:

* The client initiates the active open by sending a SYN "control" packet to the server.
* The server responds with a SYN-ACK message, which contains an acknowledgement number for the original message.
* In the third step, the client sends an ACK message back to the server to ensure that our data is being delivered reliably.

3. Now three-way handshake completed and an established connection where both the client and server have received acknowledgment of the connection from the other party.

### Step 4: Send an HTTP Request

1. The request is made up of a "request line", request header, and a body.
2. Once the HTTP request is sent, it follows a similar routing procedure.
3. Once the server receives the request, processes it, and finds the resource being requested, it generates an HTTP response.
4. Once the response is generated, the server responds to the request. At the TCP layer.

### Step 5: Tearing Down and Cleaning Up

1. Once the response has been fully delivered, the client sends a FIN packet at the TCP level, to which the server responds with an ACK, and then generally sends a FIN of its own, which the client responds to with its own ACK signal.
2. browser begins processing what data received.

## Do a Simple HTTP Request in Java

1. Creating a Request:we create an HttpUrlConnection instance
2. Adding Request Parameters
3. Setting Request Headers
4. Configuring Timeouts.
5. Handling Cookies
6. Handling Redirects
7. Reading the Response
8. Reading the Response on Failed Requests
9. Building the Full Response

## Resources used in this reading

1. [The HTTP Request Lifecycle](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-)
2. [Simple HTTP Request in Java](https://www.baeldung.com/java-http-request)
