```

   __        ___                    __
  / /_____ _/ (_)__ ________ ____  / /_
 /  '_/ _ `/ / / _ `/ __/ _ `/ _ \/ __/
/_/\_\\_,_/_/_/\_, /_/  \_,_/_//_/\__/
              /___/

```

# kaligrant - Kali linux in Vagrant

Run [Kali Linux](https://www.kali.org/) in [Vagrant](https://www.vagrantup.com/)

## How to

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
