---
layout: post
categories: exam final
title: Hands-on Final Exam
permalink: /final/final-exam/
---
## Task Instruction

1. Fork this repository https://github.com/ajcanlas-tip/sysad2-12021.git (Links to an external site.)
2. Clone your new repository in your VM https://github.com/< your username >/sysad2-12021.git
3. Create a branch named "final-exam" and checkout in that branch. 
4. Create an Ansible playbook that does the following with an input of a config.yaml file and structure inventory file.
    * Clone your prelim exam repository
    * Install and configure one enterprise service that can be installed in Debian,Centos and OpenSuse servers
    * Install and configure one monitoring tool that can be installed in Debian, Centos and OpenSuse servers (if it is a stack there should be option of different host)
    * Change Motd as "Ansible Managed by <username>"
5. push and commit your final-exam branch in the VM (no need for ansible.cfg upon pushing)
6. request a pull request from that branch in GitHub
7. For your final exam to be counted, please paste your repository link as an answer in this exam.

## Contents of Final Exam

[Repository:](https://github.com/rlucana-tip/sysad2-12021/tree/final-exam)

```
1812660/
└── final-exam
    ├── README.md
    ├── ansible.cfg
    ├── config.yaml
    ├── files
    │   ├── grafana_centos.repo
    │   ├── index.html
    │   ├── lucana_domain.conf
    │   ├── lucana_domain_centos.conf
    │   ├── lucana_domain_opensuse.conf
    │   ├── prometheus.service
    │   └── telegraf_centos.repo
    ├── inventory
    ├── playbook.yaml
    └── roles
        ├── change_motd
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── clone_prelimExam_centos
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── clone_prelimExam_debian
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── clone_prelimExam_opensuse
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── grafana_centos
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── grafana_debian
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── grafana_opensuse
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── httpd_centos
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── httpd_debian
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── httpd_opensuse
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── prometheus_centos
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── prometheus_debian
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── prometheus_opensuse
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── telegraf_centos
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        ├── telegraf_debian
        │   ├── README.md
        │   ├── defaults
        │   │   └── main.yml
        │   ├── handlers
        │   │   └── main.yml
        │   ├── meta
        │   │   └── main.yml
        │   ├── tasks
        │   │   └── main.yml
        │   ├── tests
        │   │   ├── inventory
        │   │   └── test.yml
        │   └── vars
        │       └── main.yml
        └── telegraf_opensuse
            ├── README.md
            ├── defaults
            │   └── main.yml
            ├── handlers
            │   └── main.yml
            ├── meta
            │   └── main.yml
            ├── tasks
            │   └── main.yml
            ├── tests
            │   ├── inventory
            │   └── test.yml
            └── vars
                └── main.yml

115 directories, 140 files
```

