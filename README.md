# Server-base

This repo installs most of the base stuff I usually want on most servers


## Usage

You need ansible, this was last tested with version 2.7 but it should probably work with versions as low as 2.4.

Download required roles :
```
ansible-galaxy install -f -r roles.yml
```

Then, create an inventory file containing your servers in the "inventories" directory

Finally, execute this playbook :
```
ansible-playbook -i inventories/your_inventory deploy.yml
```
(Add `-k` and/or `-K` as required if you need passwords)

## Usage / contributions

I'm not actually expecting anyone to find this useful enough to reuse it, even less to contribute.
If that happens to be the case, be my guest, though !

This repository is licensed under GPL, version 3 or any newer version.
