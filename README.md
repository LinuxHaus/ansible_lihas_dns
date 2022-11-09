# ansible_lihas_dns
Add DNS entries

Currently only handles UCS DNS servers

## Requirements

To run solo:
```
ansible-galaxy install -r requirements.yml
ansible-playbook -i localhost, dns.yml
```

## Dependencies

* lihas_variables

## Example Playbook

```
---
- hosts: '*'
  role: lihas_dns
...
```
## Tags

## Variables
* lihas_dns_type: ucs
* lihas_dns_ucs_server: name of ucs server
* lihas_dns_ucs_zone: base zone name in ucs

## Variables example
```
lihas_dns_type: ucs
lihas_dns_ucs_server: dc01.example.com
lihas_dns_ucs_zone: example.com
```
