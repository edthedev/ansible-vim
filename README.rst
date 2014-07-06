Ansible playbook for Vim
==========================

In most cases, you will want to add this repository as a submodule.::

    cd ansible-pelican
    git submodule add https://github.com/edthedev/ansible-vim.git

Then reference the playbook from within your tasks list in the main playbook.yml::

    ---
    - hosts: all
      tasks:
        - name: some other task
          shell: echo "Everythign is awesome!"
        - include: ansible-vim/vim.yml

