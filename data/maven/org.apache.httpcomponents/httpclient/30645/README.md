## Overview
[`org.apache.httpcomponents:httpclient`](http://search.maven.org/#search%7Cga%7C1%7Ca%3A%22httpclient%22)
http/conn/ssl/AbstractVerifier.java in Apache Commons HttpClient before 4.2.3 does not properly verify that the server hostname matches a domain name in the subject's Common Name (CN) or subjectAltName field of the X.509 certificate, which allows man-in-the-middle attackers to spoof SSL servers via a certificate with a subject that specifies a common name in a field that is not the CN field.  NOTE: this issue exists because of an incomplete fix for CVE-2012-5783.

## References
- [NVD](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2012-6153)