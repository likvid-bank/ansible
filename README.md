# Likvid Bank — Ansible

Ansible automation the Likvid platform team offers as meshStack building blocks.

## VM Hardening

meshStack dispatches `.github/workflows/ansible-vm-hardening.yml` when an application team attaches
the **Ansible VM Hardening** building block to a VM. The workflow runs the playbook in
`ansible-vm-hardening/` against that VM: the devsec.hardening OS and SSH baseline, then nginx
serving a landing page on `127.0.0.1` only.

Both are managed from [meshstack-hub `modules/ansible/vm-hardening`](https://github.com/meshcloud/meshstack-hub/tree/main/modules/ansible/vm-hardening)
and committed here by its backplane. Change them there; edits made here are overwritten on the
next deployment.
