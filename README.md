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

## License

BSD
