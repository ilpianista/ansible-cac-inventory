CloudAtCost inventory
=====================

This is a [dynamic inventory](https://docs.ansible.com/ansible/intro_dynamic_inventory.html)
script for Ansible which uses [CloudAtCost](http://cloudatcost.com/) APIs to generate
informations about hosts.

## Usage

Set the environment variables `CAC_API_KEY` and `CAC_LOGIN` and then invoke the script:

    $ ./cac.py -h
    usage: cac.py [-h] (--list | --host HOST)

    Produce an Ansible Inventory file based on CloudAtCost

    optional arguments:
      -h, --help   show this help message and exit
      --list       List active servers
      --host HOST  List details about the specific host

## Extra vars

It's possible to define extra vars using the `Notes` section in CloudAtCost panel.

Unfortunately that field does not support new lines, but you can use `__CAC__` as separator to specify multiple variables inline; e.g.:

    ansible_user=myuser__CAC__ansible_variable=foo__CAC__ansible_variable2=big foo

## Donate

Donations via [Liberapay](https://liberapay.com/ilpianista) or Bitcoin (1Ph3hFEoQaD4PK6MhL3kBNNh9FZFBfisEH) are always welcomed, _thank you_!

## License

BSD
