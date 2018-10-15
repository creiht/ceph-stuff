1. Copy these files into your rpc-ceph directory.
2. Edit `aio-vars.yml` and change the ip to the ip of your VM.
3. Run `./scripts/bootstrap-ansible.sh` to setup ansible.
4. Run `ceph-ansible-playbook -i aio-hosts playbooks/deploy-ceph.yml -e @aio-vars.yml`

I did this on an 8GB cloud instance with 3 CBS volumes.
