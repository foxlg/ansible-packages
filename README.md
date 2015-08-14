packages
=========

Ansible Role to install packages

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: zerotao.packages
           packages: # list of packages to install
             - tmux
             - vim
           remove_package: # list of packages to remove
             - build-essential
           repos:  # list of repositories to add for the packages
             - name: erlang
               repo: "deb http://packages.erlang-solutions.com/ubuntu trusty contrib"
               key: "http://packages.erlang-solutions.com/ubuntu/erlang_solutions.asc"

License
-------

BSD

