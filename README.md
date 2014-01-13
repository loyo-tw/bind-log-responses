bind-log-responses
==================

Patch for ISC Bind(named) used for log DNS request's responses.
This patch will make named to log DNS reply messages to its query log file.
NOTE:
Log response message might slow down your DNS Server and the performance, use it after you know what it is doing.

Install
-------
- Patch File
`/bin/gpatch -p0 -i bind993p2-log-responses.patch`

Usage
-----
In named.conf
###	
	option {
		...
		log-responses  yes|no;
		...
	}
* log-responses yes: Enable log responses.
* log-responses no: Disable log responses. 

Author
------
Loyo Fulamce 


