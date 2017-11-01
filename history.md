    1  ls
    2  pwd
    3  git clone https://github.com/yosephabate/eduroam_radius
    4  ls
    5  cd eduroam_radius/
    6  ls
    7  cp inventories/template inventories/ubuntunet.net
    8  exit
    9  ls
   10  rm -r eduroam_radius/
   11  ls
   12  git clone https://github.com/ubuntunet/eduroam_radius.git
   13  ls
   14  cd eduroam_radius/
   15  ls
   16  cp inventories/template inventories/aait_edu_et
   17  code .
   18  cd
   19  sudo apt-get update
   20  sudo apt-get install code
   21  curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
   22  sudo mv microsoft.gpg /etc/apt/trusted.gpg.d/microsoft.gpg
   23  sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'
   24  sudo apt-get install code
   25  cd eduroam_radius/
   26  vim inventories/aait_edu_et 
   27  cp group_vars/template group_vars/aait_edu_et
   28  vim group_vars/aait_edu_et 
   29  cp group_vars/clients.yml.example group_vars/clients.yml
   30  vim group_vars/clients.yml
   31  vp group_vars/secrets.yml.example group_vars/secrets.yml
   32  vim group_vars/secrets.yml.example group_vars/secrets.yml
   33  ansible-playbook -i inventories/aait_edu_et eduroam_idp.yml 
   34  cp group_vars/secrets.yml.example group_vars/secrets.yml
   35  vim group_vars/secrets.yml
   36  ansible-playbook -i inventories/aait_edu_et eduroam_idp.yml 
   37  ansible-playbook -i inventories/aait_edu_et -c local eduroam_idp.yml 
   38  vim inventories/aait_edu_et 
   39  ansible-playbook -i inventories/aait_edu_et -c local eduroam_idp.yml 
   40  vim inventories/aait_edu_et 
   41  ansible-playbook -i inventories/aait_edu_et -c local eduroam_idp.yml 
   42  vim roles/freeradius/tasks/install.yml 
   43  edit
   44  exit
   45  cd eduroam_radius/
   46  vim group_vars/clients.yml
   47  ansible-playbook -i inventories/et_aait eduroam_idp.
   48  ansible-playbook -i inventories/et_aait eduroam_idp.yml 
   49  ansible-playbook -i inventories/et_aait -c local eduroam_idp.yml 
   50  vim group_vars/clients.yml
   51  ls -F group_vars/
   52  vim group_vars/et_aait 
   53  radtest roamer abc123 127.0.0.1:1812 0 testing123
   54  sudo vim /etc/hosts
   55  sudo service networking restart
   56  radtest roamer abc123 127.0.0.1:1812 0 testing123
   57  history
   58  history > history.md
