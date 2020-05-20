# DevOps_Spring_2020 answer

dkop@dkop-VirtualBox:~/GIT$ ansible-playbook HW_Ansible.yml 

PLAY [Install differents web_servers] ********************************************************************************************************

TASK [Gathering Facts] ***********************************************************************************************************************
ok: [10.0.2.7]
ok: [10.0.2.9]

TASK [Check and Print Linux Version] *********************************************************************************************************
ok: [10.0.2.9] => {
    "ansible_os_family": "Debian"
}
ok: [10.0.2.7] => {
    "ansible_os_family": "RedHat"
}

TASK [Install Apache For Debian] *************************************************************************************************************
skipping: [10.0.2.7]
ok: [10.0.2.9]

TASK [Copy my web site] **********************************************************************************************************************
skipping: [10.0.2.7]
ok: [10.0.2.9]

TASK [Start Web Server for Debian] ***********************************************************************************************************
skipping: [10.0.2.7]
ok: [10.0.2.9]

TASK [Check that you can connect (GET) to a page and it returns a status 200] ****************************************************************
skipping: [10.0.2.7]
ok: [10.0.2.9]

TASK [Check that a page returns a status 200 and fail if the word Playbook is not in the page contents] **************************************
skipping: [10.0.2.7]
ok: [10.0.2.9]

TASK [Install Nginx web Server for RedHat] ***************************************************************************************************
skipping: [10.0.2.9]
ok: [10.0.2.7]

TASK [Copy my web site] **********************************************************************************************************************
skipping: [10.0.2.9]
ok: [10.0.2.7]

TASK [Start Web Server for RedHat] ***********************************************************************************************************
skipping: [10.0.2.9]
ok: [10.0.2.7]

TASK [Check that you can connect (GET) to a page and it returns a status 200] ****************************************************************
skipping: [10.0.2.9]
ok: [10.0.2.7]

TASK [Check that a page returns a status 200 and fail if the word Playbook is not in the page contents] **************************************
skipping: [10.0.2.9]
ok: [10.0.2.7]

PLAY RECAP ***********************************************************************************************************************************
10.0.2.7                   : ok=7    changed=0    unreachable=0    failed=0   
10.0.2.9                   : ok=7    changed=0    unreachable=0    failed=0 
