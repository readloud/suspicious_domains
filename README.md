# suspicious_domains
 There are several malware websites or domains on the internet that may contain spam or malware.

## Automatic close domain name variant detection using string similarities

Phishing, as one of the most popular social engineering attacks, aims to obtain an Internet user’s personal information through a phony website that looks like a legitimate site, or by sending a phishing email. Such attacks are causing serious damages and losses. 

## The scope
There are several approaches to convincing an Internet user that a domain name or website is legitimate or looks like a popular brand. Take this URL as an example: http://paypal.com-security.active-userid.com. Although the real domain name is active-userid.com, one can make the domain look like paypal.com by adding subdomains. In our case, since the data we are using is only the domain name (e.g., domain.co.nz) part of the URL, which can only be set once at registration, our approach aims to detect the close domain name variant cases summarized in the table below:

|Type of varient|Example|
|---------------|-------|
|Missing dot|wwwpaypal.co.nz
|Char omission, permutation, substitution|payspal.co.nz|
|combo using '-'|www-secure-paypal.co.nz|
|Add/change second level|paypal.ac.nz|
|Homograph|paypa1.co.nz|
|Homophone|paypaw.co.nz|
 
That is, the cases where a domain name seems normal (i.e. it is not close variant to any popular domain/brand) but is used for other purposes, are outside the scope of this research project.
