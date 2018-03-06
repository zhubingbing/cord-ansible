```
## Deploy onos and xos

ansible-playbook -i inventory/multinode -e @../etc/global.yml -e action=deploy site.yml

## Generate openstack-compute-vtn configuration file

ansible-playbook -i inventory/multinode -e @../etc/global.yml compute-node-enable-playbook.yml

## Onboard openstack vtn onos in xos

ansible-playbook -i inventory/multinode -e @../etc/global.yml cord-improve.yaml

```
