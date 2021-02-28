# Setup and Deploy Traefik For Local Docker Containers

To run against the local machine named bolivar. NOTE: To get Lets Encrypt to work (and so I can access the machine remotely) my local machine is set up to be accessible from the internet as bolivar.kedrovsky.com.

    ansible-playbook -i inventory.bolivar -u root -K --connection=local --ask-vault-pass playbook.yml

To run against remote remote server with a hostname of "linode-web01-2004". This assumes a SSH key has been uploaded to your Linode profile.

    ansible-playbook -i inventory.linode -u root --ask-vault-pass playbook.yml
