This is a small home lab I put together to see how Windows event logs flow through a SIEM in a real environment. 

The setup includes a Windows Domain Controller, a Windows test machine, and a Splunk Enterprise server running on Ubuntu. Once everything was connected inside a Vultr VPC, I started forwarding Security logs from the Windows hosts into Splunk to see authentication activity and system events in real time.
A simple setup to understand AD, logging, forwarding, and how SIEMs actually ingest and display telemetry.

Components:

-A domain controller (Heeruzen-ADDC01) managing a small test domain

-A Windows server joined to the domain

-Splunk Enterprise running on Ubuntu

-Universal Forwarder set up to ship Security logs

-Basic indexing and log searches

-A private VPC network holding everything together
