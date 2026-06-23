# kubernetes
Ansible role to setup a Kubernetes cluster.

Installs the following packages (see version in defaults/main.yml):
- containerd
- runc

Playbook example:

---

- name: Install and configure Kubernetes
  hosts: kubernetes
  become: yes

  roles:
    - kubernetes

...
