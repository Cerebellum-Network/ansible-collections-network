# DDC Gateway configuration

## Usage

Playbook

```yaml
---
- name: Prepare OS configuration for DDC deployment
  hosts: all
  remote_user: root
  roles:
    - cere.network.common

- name: Deploy latest application
  hosts: ddc-gateway-devnet,ddc-gateway-testnet,ddc-gateway-mainnet
  remote_user: root
  roles:
    - cere.network.ddc_gateway
```

Expected configuration:
