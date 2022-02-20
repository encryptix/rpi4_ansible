Uses a python env called 'ansible'
python3.8 -m venv ansible
install ansible
Ansible then has two additional installs:
- ansible-galaxy install geerlingguy.docker_arm
- ansible-galaxy collection install community.general

Using vscode, can select the interpretor
Manually, source ansible/bin/activate ... then run deactivate when done

ansible-playbook rpi-4.yml -i hosts

# After setup of a generic home assistant, there are some specific settings in another play:
ansible-playbook home_assistant_02.yml