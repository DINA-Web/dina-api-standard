This document
=============

DRAFT


Background
=============
This document sets out a set of policies with respect to IT security and DINA software.

The DINA TC views secure software as fundamental to the integrity of DINA-produced software, also supporting the confidence of partners adopting DINA software.

Some definitions:
* Security: availability, integrity and confidentiality


Summary
=============
* 'https' everywhere
* Applications and web services pass OWASP10
* Non-DINA components hardened as-per component best-practices
* docker hardening


http/https
==========
All applications and web services are to run only 'https'.


Web application and Web Services Security
=============
Web applications (including web services like a RESTful web service) must test the application or service with the Open Source tool, (OWASP ZED)[https://www.owasp.org/index.php/OWASP_Zed_Attack_Proxy_Project].

For each release, for each web application/service:
* Will have a directory called 'security' which will contain the OWASP ZED HTML report *for that release of the application/service*.
* Other security controls (below) will also be in the 'security' directory
* TODO: agree on what tool to use

ToolsContinuous Integration
----------------------
* (Jenkins plugin)[https://wiki.jenkins-ci.org/display/JENKINS/Zapper+Plugin]
* (OWASP Dependency-Check)[OWASP Dependency-CheckOWASP Dependency-Check] -- (Jenkins plugin)[https://wiki.jenkins-ci.org/display/JENKINS/OWASP+Dependency-Check+Plugin]
* (OWASP Lapse Project)[https://www.owasp.org/index.php/OWASP_LAPSE_Project]





Dependent Component Security
=============
Applications/services depend on non-DINA applications/services for operation.
An example is a datqabase like MySql or Postgresql.

Application/service dependencies/components should adhere to the security best practices for that component.
For example, MySql can be secured or *hardened* using guidelines such as (MySQL Database Security Best Practices)[http://www.greensql.com/content/mysql-security-best-practices-hardening-mysql-tips].

Components may be deployed and configured by the end users or by DINA scripts.
In either case, a desciption of all of the security controls put in place, or required to put in place, to harden the component should also be in the 'security' directory.
(An example security directory is forthcoming).

docker hardening
================
As docker is a fundamental technology for this project, making it secure is a priority.
* (docker hardening - 1.6)[https://benchmarks.cisecurity.org/tools2/docker/CIS_Docker_1.6_Benchmark_v1.0.0.pdf]
* Install (fail2ban)[http://www.fail2ban.org/]










