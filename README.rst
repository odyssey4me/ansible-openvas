Ansible OpenVAS
###############
.. image:: https://travis-ci.org/odyssey4me/ansible-openvas.svg?branch=master
    :target: https://travis-ci.org/odyssey4me/ansible-openvas
.. image:: https://img.shields.io/badge/license-Apache%202.0-brightgreen.svg?style=flat
    :target: http://opensource.org/licenses/apache-2.0

:tags: openvas, security, ansible
:category: \*nix

Role for the deployment of the OpenVAS Scanner, Manager and CLI.

Example Ansible play

.. code-block:: yaml

    - name: Install OpenVAS Server
      hosts: openvas_all
      user: root
      roles:
        - { role: "openvas_server", tags: [ "openvas-scanner", "openvas-manager", "openvas-cli" ] }
      vars:
        openvas_admin_password: secrete

Warning: This is a Proof of Concept at this stage, nothing more. Use at your own risk.
