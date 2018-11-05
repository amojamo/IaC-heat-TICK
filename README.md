# Heat Template used for deploying TICK-stack - Forked from [githubgossin](https://github.com/githubgossin/IaC-heat-k8s)

This is a Heat template to launch a TICK-stack, for a project in IMT3005 IaC. The servers are initialized based on [this Puppet control repo](https://github.com/amojamo/imt3005tick).

The stack is deployed using the following commands:
```bash
# Make sure you have security groups called default and linux.
# Edit iac_top_env.yaml and enter name of your keypair.
# After running the openstack stack create command, 
# wait at least 15 minutes for everything to get up and running.
git clone https://github.com/githubgossin/IaC-heat-k8s.git
cd IaC-heat-k8s
openstack stack create k8s-lab -t iac_top.yaml -e iac_top_env.yaml
```
Access Chronograf through your browser at http://*floatingip*:8888
