common-lae
=========

Common configuration for all machines maintained by Musee

Role Variables
--------------

|Name|Type|Description|Default|
|----|----|-----------|-------|
`ntp_servers`|List|NTP servers to sync to|[sca-ntp1.eng.fireeye.com, sca-ntp2.eng.fireeye.com, sca-ntp3.eng.fireeye.com]
`common_packages`|List|OS Packages to install|[ngrep]

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - { role: common, common_packages: [ 'ngrep' ] }
