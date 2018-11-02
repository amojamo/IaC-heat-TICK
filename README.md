# Pending

This is a Heat template to launch a Kubernetes lab exercise. The servers are initialized based on [this Puppet control repo](https://github.com/githubgossin/control-repo-k8s).

Clone and launch in OpenStack with e.g.
```bash
# make sure you have security groups called default and linux
# edit iac_top_env.yaml and enter name of your keypair
git clone https://github.com/githubgossin/IaC-heat-k8s.git
cd IaC-heat-k8s
openstack stack create k8s-lab -t iac_top.yaml -e iac_top_env.yaml
```
## Troubleshooting
+ [debug...](https://www.rabbitmq.com/troubleshooting-ssl.html)
