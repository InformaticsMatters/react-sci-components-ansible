# React Mini-Apps (Ansible)

[![Build Status](https://travis-ci.com/InformaticsMatters/website-ansible.svg?branch=master)](https://travis-ci.com/InformaticsMatters/website-ansible)

A playbook and Role to deploy the [Mini-Apps] website application, suitable for
execution by [AWX].

This project contains one Ansible role:-

*   **mimi-apps**

>   Note: The Role is designed to be executed from within our AWX server
    where credentials for the cluster (Kubernetes) reside. If you're not
    running from AWX (discouraged) then you will need to provide
    values for the variables that would be injected by AWX.

We depend on our [infrastructure] project's Kubernetes
**Certificate Manager** to generate https certificates.

As with all of our playbooks you can find the common user-defined variables
in the role's `defaults/main.yaml` and less common variables in
`vars/main.yaml`.

---

[awx]: https://github.com/ansible/awx
[infrastructure]: https://github.com/InformaticsMatters/ansible-infrastructure
[mini-apps]: https://gitlab.com/informaticsmatters/react-sci-components