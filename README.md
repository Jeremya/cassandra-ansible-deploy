# cassandra-ansible-deploy
Ansible playbooks to deploy Cassandra cluster

Fill the hosts file with your server's ip
Run it using `ansible-playbook master_deploy_cluster.yaml -i hosts --private-key=<path to ssh key>`

# TODO
  * Check Cassandra is installed before configuring it
  * Configure listen_address: private_ip & rpc_address: public_ip
  * Refactor racks management
  * Implement rack distribution
  * Token range distribution imbalanced ==> implement allocate_tokens_for_keyspace
  * Write a Readme
