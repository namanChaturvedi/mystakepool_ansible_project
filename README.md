# mystakepool_ansible_project (Refer RAW text form of this file)
This project sets up 1 core, 1 relay and 1 service node for Cardano stake pool setup

This project has been used for experimental setup, and can't be established as source to particular design protocol. Users are free to utilize this project for their personal interest/setup.  

Project structure for Initial setup is "first_setup"

├── ansible.cfg
├── first_setup.yml
├── hosts
└── roles
    ├── bp_node (name differ to actual dir_name)
    │   ├── handlers
    │   │   └── main.yml
    │   ├── tasks
    │   │   └── main.yml
    │   └── vars
    │       └── main.yml
    ├── build_cardano_project
    │   ├── handlers
    │   ├── tasks
    │   │   └── main.yml
    │   └── vars
    │       └── main.yml
    ├── common
    │   ├── files
    │   │   └── apt_periodic
    │   ├── handlers
    │   │   └── main.yml
    │   ├── tasks
    │   │   └── main.yml
    │   └── vars
    │       └── main.yml
    ├── relay_node (name differ to actual dir_name)
    │   ├── handlers
    │   │   └── main.yml
    │   ├── tasks
    │   │   └── main.yml
    │   └── vars
    │       └── main.yml
    └── servicenode
        ├── files
        │   ├── jail.local
        ├── handlers
        │   └── main.yml
        ├── tasks
        │   └── main.yml
        └── vars
            └── main.yml

# Playbook to run Initial Setup --> /first_setup/first_setup.yml (configure your hostname in "hosts" file)
#                       command --> ansible-playbook -K first_setup.yml
