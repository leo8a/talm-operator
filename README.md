# Ansible Role: TALM operator

[![CI](https://github.com/leo8a/talm_operator/actions/workflows/ci.yml/badge.svg)](https://github.com/leo8a/talm_operator/actions/workflows/ci.yml)

Installs the [TALM](https://github.com/openshift-kni/cluster-group-upgrades-operator.git) operator on OpenShift clusters.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    talm:
      install_method: "olm"                    # -> available options: olm, source

## Dependencies

This role requires the `kubernetes.core` collection, and have been tested on an OpenShift cluster version 4.10.

## Example Playbook

    - hosts: localhost
      gather_facts: false
      roles:
        - leo8a.talm_operator

## License

This role is released under the Apache 2.0 license. See the [LICENSE](LICENSE).

## Author Information

This role was created in 2022 by [Leo Ochoa](https://github.com/leo8a/).

## Contributors

This is the current list of folks in the `talm_operator` hall of ~~fame~~ contributors 🏆!

<a href="https://github.com/leo8a/talm-operator/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=leo8a/talm-operator"  alt=""/>
</a>

> Made with [contributors-img](https://contrib.rocks).
