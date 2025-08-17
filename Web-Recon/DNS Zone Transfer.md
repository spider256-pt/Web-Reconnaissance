1. DNS zone transfer is essentially a wholesale copy of all DNS records within a zone from one name server to another.
2. If not configured correctly hen it can reveal complete list of subdomains, their associated IP address and other sensitive DNS data.
##### Process of zone transfer:
1. Zone Transfer Request(AXFR): The secondary server initiates the process by sending a zone transfer request.
2. SOA Record Transfer: After the AXFR is done then the primary server responds it with SOA {Strat of Authority} record.
3. DNS Recodes Transmission: The primary rec then transfer all DNS records in the zone to the secondary server.
4. Zone Transfer Complete: Once all record have been transmitted, the primary server signals the end of the zone transfer.
5. The secondary server sends an acknowledgement message to the primary server, confirming the successful receipt and processing of the zone data.
#### Zone transfer Vulnerability

1. The information gleaned from an unauthorized zone transfer can be invaluable to an attacker.
2.  It reveals a comprehensive map of the target's DNS infrastructure, including:
	1. Subdomains
	2. IP Addresses
	3. Name Server Records

## Exploit Zone Transfers:

###### Command:
	dig axfr @<name_Server_ip/hostname> <name_server>


[[DNS{Domain Name System}]]