/*
Title: Tomcat Manager - Default Login Credentials
Description: Search engine meta data about the finding
*/

- LAST UPDATED DATE: 2015/11/25
- LAST UPDATED BY: @mubix

## Summary

Default Tomcat Management credentials  

## Capabilities and Risk

This is to replace any "level" or "score" becuase of how much context is needed
for a vulnerability to have one which is beyond the scope of this database.

- List of possible uses for this vulnerability to give real-world uses
- Read files as www-data (or use web server is running as)
- DDoS service
- Code execution (for this one to fly there needs to be a refence proving it) 

## Detection

Default credentials can be tried by authenticating witht the http Tomcat login. The list below contains default Tomcat credentials.

**username/password**
- tomcat/tomcat
- both/tomcat
- role1/tomcat
- manager/manager
- admin/admin


## Remediation

Default accounts should be disabled or have their password reset.

## References

- Link to blog post
- Link to CVE
- Link to Metasploit module
- Link to Nessus/NeXpose/Qualys write up

## Exploitation

The tomcat management console can be accessed by navigating to the url: http://x.x.x.x:8080/manager
