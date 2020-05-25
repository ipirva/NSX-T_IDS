# NSX-T IDS with Network Container Plugin

The repository contains the Kubernetes manifests for the deployment of an old Drupal (7.0), PHP (5.6), MySQL (5.0) setup.
Drupal 7.0 container image is built from the provided Dockerfile.

There are some CVEs that will trigger alarms on the IDS:

- MySQL DELETE tbl_name heap buffer overflow (CVE-2012-5612)
- Drupal 7 Preauth SQL Injection (CVE-2014-3704)
- ET WEB_SPECIFIC_APPS [PT OPEN] Drupalgeddon2 <8.3.9 <8.4.6 <8.5.1 RCE Through Registration Form (CVE-2018-7600)
- MySQL/MariaDB memcmp() SSE authentication bypass (CVE-2012-2122)
