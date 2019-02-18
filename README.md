# ansible
ansible playbook

The playbook purposes to
1. deploy Red Hat OpenJDK to managed Windwos hosts
2. set JAVA_HOME
3. add %JAVA_HOME%\bin to PATH
4. print the result of 'java.exe -version' to console

To run the playbook, you must
- manually save the OpenJDK installer (a zipped file) from Red Hat. This requires authentication.
- upload the OpenJDK installer to filesystem of ansible
- edit the playbook to update the paths in ansible and windows
- create an inventory host group called windows
- it generally require local admin rights to update environmental variables
