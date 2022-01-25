# ansible-role-weka
Basic ansible role to install weka


## Usage

This role expects an API token to communicate with weka to download the relevant install scripts etc. This API token can be found at https://get.weka.io/ui/account/api-tokens. It should be inserted into your playbook run via

```
ansible-playbook -i inventories/k8s/hosts.yaml k8s.yml -k --tag weka --limit sdfk8s001.slac.stanford.edu --extra-vars "weka_api_token=XXXXXXXX"
```

We should probably put the token into a (hashicorp) vault and integrate into ansible.


