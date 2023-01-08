# docker-vpn

# На стороне клинета 

ssh-copy-id root@<remote_host>

# На стороне сервера

sudo nano /etc/ssh/sshd_config

+- PasswordAuthentication no --> yes

++ PubkeyAuthentication yes
++ ChallengeResponseAuthentication no


sudo systemctl reload ssh
