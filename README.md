andrelohmann.grafana_oss
========================

Install grafana-oss from apt repository

  * https://grafana.com/docs/grafana/latest/installation/debian/#install-from-apt-repository

<!---

!!!This will be necessary, when Ansible 2.10 gets released

Role Dependencies
-----------------

This role depends on the community.general collection. Add the following to your requirements.yml:

    ---
    roles:
    - andrelohmann.grafana_oss
    collections:
    - community.general # a dependency for the andrelohmann.grafana_oss role
    ...

--->

Role Variables
--------------

    grafana_additional_configs:
    - section: null
      option: app_mode
      value: production
    - section: server
      option: http_addr
      value: 0.0.0.0
    - section: server
      option: http_port
      value: 3000

Example Playbook
----------------

    - hosts: grafana
      roles:
      - andrelohmann.grafana_oss

License
-------

MIT

Author Information
------------------

https://github.com/andrelohmann
