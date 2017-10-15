this repo is to illustrate the difference in how ansible handles hostvars.

`vagrant up` and `vagrant provision` runs one host at a time, so hostvars files from other hosts are not read.

After vagrant up do:

1. `ansible-playbook test.yml`
2. `ansible-playbook test.yml -l ws-a -check -D`
