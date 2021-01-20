---
layout: post
categories: exam midterm
title: Hands-on Midterm Exam
permalink: /midterm/midterm-exam/
---
## Task Instruction

1. Fork this repository https://github.com/ajcanlas-tip/sysad2-12021.git (Links to an external site.)
2. Clone your new repository in your VM https://github.com/< your username >/sysad2-12021.git
3. Create a branch named "midterm-exam" and checkout in that branch. 
4. Create an Ansible playbook that does the following with an input of a config.yaml file and arranged Inventory file:
    * 4.1 Install and configure Elastic Stack in separate  hosts (Elastic Search, Kibana, Logstash)
    * 4.2 Install Nagios in one host
    * 4.3 Install Grafana,Prometheus and Influxdb in seperate hosts (Influxdb,Grafana,Prometheus)
    * 4.4 Install Lamp Stack in seperate hosts (Httpd + Php,Mariadb)
5. push and commit your midterm-exam branch in the VM (no need for ansible.cfg upon pushing)
6. request a pull request from that branch in GitHub
7. For your midterm exam to be counted, please paste your repository link as an answer in this exam.

## Contents of Midterm Exam

[Repository:](https://github.com/rlucana-tip/sysad2-12021/tree/midterm-exam)

```
1812660/
└── midterm-exam
    ├── README.md
    ├── ansible.cfg
    ├── files
    │   ├── index.html
    │   ├── lucana_domain.conf
    │   └── prometheus.service
    ├── inventory
    ├── playbook.yaml
    └── roles
        ├── elasticSearch
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
        ├── grafana
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
        ├── httpd_php
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
        ├── influxdb
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
        ├── kibana
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
        ├── logstash
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
        ├── mariadb
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
        ├── nagioscore
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
        └── prometheus
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

66 directories, 79 files
```

