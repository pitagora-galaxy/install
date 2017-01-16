# Pitagora-Galaxy 0.3.2

## Installation

The scripts are tested on Ubuntu 14.04.4.
* AWS: ubuntu-trusty-14.04-amd64-server-20160114.5 (ami-a21529cc)

Install Git and clone this repository.
* Set MySQL password to 'galaxy' when its prompt asks.
```
$ sudo apt-get update
$ sudo apt-get install -y git
$ git clone https://github.com/pitagora-galaxy/install-0.3.2.git
```

Install OS Packages, Python, Galaxy.
```
$ cd scripts
$ sh 01_install.sh
..
serving on http://127.0.0.1:8080
(Ctl + C to exit)
```

Configure Galaxy installation (database, disks, proxy, etc.)
```
$ cd scripts
$ sh 02_config.sh
```

Install Galaxy tools from ToolShed or from GitHub.
```
$ cd scripts
$ sh 03_tools.sh
```

Import Pitagora's workflows.
```
$ cd scripts
$ sh 04_workflows.sh
```

## Workflows

* For the details of workflows, see our [wiki](http://wiki.pitagora-galaxy.org/wiki/index.php/Workflows).
