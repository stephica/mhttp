# mHTTP
In today’s Internet, one of the main detriments in user experience is completion times of data transfers that for large objects is limited by network capacity. However, recent developments have opened new opportunities for reducing end-to-end latencies. First, most end-user devices have multiple network interfaces (i. e., interface diversity). Second, popular contents are often available at multiple locations in the network (i. e., data source diversity). When combined, these provide substantial path diversity within the Internet that can be used by users to improve their quality of experience.

Multi-source Multipath HTTP (mHTTP) enables users to establish simultaneous connections with multiple servers to fetch a single content. mHTTP is designed to combine the advantage obtained from distributed network infrastructures provided by CDNs with the advantage of multiple interfaces at end-users. Unlike existing proposals: a) mHTTP is a purely receiver-oriented mechanism that requires no modification either at the server or at the network, b) the modifications are restricted to the socket interface; hence, no changes are needed to the applications or to the kernel, and c) it takes advantage of multiple types of path diversity in the Internet.

The mHTTP design consists of: (i) multiHTTP: a set of modified socket APIs which splits content into multiple chunks, requests each chunk via individual HTTP range requests from the available servers, reassembles the chunks and delivers the content to the application. (ii) multiDNS: a modified DNS resolver that obtains IP addresses for a server name by harvesting the DNS replies and/or by performing multiple lookups of the same server name by contacting different domain name servers.
