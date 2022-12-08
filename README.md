# Red Hat OpenShift Service Mesh: Traffic Management Labs

## Introduction

The objective of these labs is to get a deep understanding of the following topics:

- Smart traffic routing, shifting and mirroring.
- Ingress and Egress
- Fault Injection
- Fault Tolerance and Circuit Breaking
- gRPC routing

## Tutorial documentation

These labs have been created using asciidoc and include a setup script to create and publish a binary container image to run and serve the resulting html.

They can be used in any OpenShift 4 cluster but a script is provided to install an AWS IPI cluster using OPENTLC.

Please follow the next procedure to deploy these labs in OpenShift:

- Complete `ocp4-aws-install/config.env` file with correct values
- Setup users in `ocp4-aws-install/users.txt`
- Execute the following commands in the bastion host provided by OPENTLC:

```$bash
./ocp4-aws-install/ocp4-aws-install.sh ocp4-aws-install/config.env
```

- Complete `deploy-lab-docs/config.env` file with correct values
- Execute the following commands in any host with `oc` command:

```$bash
./deploy-lab-docs/deploy.sh
```

## Author Information

- Ignacio Sánchez (isanchez@redhat.com)
- Ernesto González (ergonzal@redhat.com)
