=============================
watchguard-letsencrypt-deploy
=============================
expect script for deploy letsencrypt certificates to WatchGuard Firewalls


How to use:
the expect script use the WatchGuard SSH API to install certificates.

run push-root-ca.sh to deploy the root CA.

run push-sub-ca.sh to deploy the sub CA.

run push-le-cert.sh to deploy your certificate with private key.

optional you can add your own certificates with push-single-cert.sh

Download
--------

* `github repository <https://github.com/watchguard-toolbox-project/watchguard-letsencrypt-deploy/>`_
