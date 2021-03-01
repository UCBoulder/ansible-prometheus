# Ansible Collection - cub_oit_pe.prometheus

I'd recommend anyone from the the public looking at this in Ansible Galaxy NOT use this collection.
This has mainly been built as a learning expirement. Though it is functional for our needs, it is
not meant to be featureful and cover all use cases.

Consider (cloudalchemy/prometheus)[https://galaxy.ansible.com/cloudalchemy/prometheus] instead.

### How to run tests locally

* Requires podman with RHEL entitlement

```sh
export REPO=$(pwd)
cd ~/.ansible/collections/ansible_collections
mkdir cub_oit_pe
cd cub_oit_pe
ln -s $REPO prometheus
cd $REPO/tests/integration
molecule -c molecule/base.yml test --all
```