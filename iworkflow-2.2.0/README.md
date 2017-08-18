# iWorkflow-2.2.0.0.0.10548 Vagrant box

This Vagrantfile can be used to start a iWorkflow vagrant box for version 2.2.0.

## Requirements

This Vagrantfile requires that following be installed on the machine the
vagrant command is run on.

  * Virtualbox
  * Vagrant
  * A valid license for iWorkflow

## Usage

After creating a Vagrant box using the associated packer file found
[here](https://github.com/f5devcentral/f5-packer-templates/tree/master/iworkflow-2.2.0-x86_64-box),
take the created box 

  * iWorkflow-2.2.0.0.0.10548.box

and place it in this directory alongside the Vagrantfile.

Next, run the following command

  IWF_LICENSE=xxxx-xxxx-xxxx-xxxx-xxxxxxx vagrant up

and wait for it to finish. The resulting instance of BIG-IP will be
available via CLI and Web UI

## Connecting

To connect to the CLI, use either `vagrant ssh`, or open the VM in Virtualbox
by double clicking its entry in the list of VMs

To connect to the web UI, follow this link

  * https://localhost:10443/
