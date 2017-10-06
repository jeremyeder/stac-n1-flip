# Automation to flip between bare metal and kubernetes-based STAC-A2 configurations.

# Usage

## Clone this git repo
```
# git clone https://github.com/jeremyeder/stac-n1-flip
```

Starting/Stopping the Kubernetes configuration is done by setting the baremetal variable to True or false.

## Disable Kubernetes:
```
# ansible-playbook -v -i inventory/stac-n1.inv playbooks/stac-n1-flip.yaml --extra-vars "baremetal=True"
```

## Enable Kubernetes:
```
# ansible-playbook -v -i inventory/stac-n1.inv playbooks/stac-n1-flip.yaml --extra-vars "baremetal=False"
```
