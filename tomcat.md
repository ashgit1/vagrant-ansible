
PLAY [tomcat-servers] **********************************************************************************************************************************************************

TASK [Gathering Facts] *********************************************************************************************************************************************************
ok: [192.168.33.20]
ok: [192.168.33.10]

TASK [selinux : Download EPEL Repo - Centos/RHEL 6] ****************************************************************************************************************************
skipping: [192.168.33.10]
skipping: [192.168.33.20]

TASK [selinux : Install EPEL Repo - Centos/RHEL 6] *****************************************************************************************************************************
skipping: [192.168.33.10]
skipping: [192.168.33.20]

TASK [selinux : Download EPEL Repo - Centos/RHEL 7] ****************************************************************************************************************************
ok: [192.168.33.10]
ok: [192.168.33.20]

TASK [selinux : Install EPEL Repo - Centos/RHEL 7] *****************************************************************************************************************************
ok: [192.168.33.10]
ok: [192.168.33.20]

TASK [selinux : Install libselinux-python] *************************************************************************************************************************************
ok: [192.168.33.10]
ok: [192.168.33.20]

TASK [tomcat : Install Java 1.7] ***********************************************************************************************************************************************
ok: [192.168.33.10]
ok: [192.168.33.20]

TASK [tomcat : add group "tomcat"] *********************************************************************************************************************************************
ok: [192.168.33.20]
ok: [192.168.33.10]

TASK [tomcat : add user "tomcat"] **********************************************************************************************************************************************
ok: [192.168.33.20]
ok: [192.168.33.10]

TASK [tomcat : Download Tomcat] ************************************************************************************************************************************************
ok: [192.168.33.10]
ok: [192.168.33.20]

TASK [tomcat : Extract archive] ************************************************************************************************************************************************
ok: [192.168.33.10]
ok: [192.168.33.20]

TASK [tomcat : Symlink install directory] **************************************************************************************************************************************
ok: [192.168.33.10]
ok: [192.168.33.20]

TASK [tomcat : Change ownership of Tomcat installation] ************************************************************************************************************************
ok: [192.168.33.10]
ok: [192.168.33.20]

TASK [tomcat : Configure Tomcat server] ****************************************************************************************************************************************
ok: [192.168.33.20]
ok: [192.168.33.10]

TASK [tomcat : Configure Tomcat users] *****************************************************************************************************************************************
ok: [192.168.33.10]
ok: [192.168.33.20]

TASK [tomcat : Install Tomcat init script] *************************************************************************************************************************************
ok: [192.168.33.10]
ok: [192.168.33.20]

TASK [tomcat : Start Tomcat] ***************************************************************************************************************************************************
ok: [192.168.33.10]
ok: [192.168.33.20]

TASK [tomcat : deploy iptables rules] ******************************************************************************************************************************************
skipping: [192.168.33.10]
skipping: [192.168.33.20]

TASK [tomcat : insert firewalld rule for tomcat http port] *********************************************************************************************************************
changed: [192.168.33.20]
changed: [192.168.33.10]

TASK [tomcat : insert firewalld rule for tomcat https port] ********************************************************************************************************************
changed: [192.168.33.10]
changed: [192.168.33.20]

TASK [tomcat : wait for tomcat to start] ***************************************************************************************************************************************
ok: [192.168.33.20]
ok: [192.168.33.10]

PLAY RECAP *********************************************************************************************************************************************************************
192.168.33.10              : ok=18   changed=2    unreachable=0    failed=0   
192.168.33.20              : ok=18   changed=2    unreachable=0    failed=0   

