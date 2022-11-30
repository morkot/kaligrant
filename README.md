```

 _         _ _                       _
| |       | (_)                     | |
| | ____ _| |_  __ _ _ __ __ _ _ __ | |_
| |/ / _` | | |/ _` | '__/ _` | '_ \| __|
|   < (_| | | | (_| | | | (_| | | | | |_
|_|\_\__,_|_|_|\__, |_|  \__,_|_| |_|\__|
                __/ |
               |___/

```

# kaligrant - Kali linux in Vagrant

Run [Kali Linux](https://www.kali.org/) in [Vagrant](https://www.vagrantup.com/)

## How to use

Quick start:

```shell
vagrant up --provision
```

Just to start the virtual machine:

```shell
vagrant up
```

To apply configuration defined in ansible:

```shell
vagrant provision
```

To upgrade the system with latest packages (takes quite long time):

```shell
KALIGRANT_UPGRADE=true vagrant provision
```

## Contribute

Submit and issue or PR in a free form.
