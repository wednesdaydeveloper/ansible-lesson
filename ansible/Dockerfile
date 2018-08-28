FROM ansible/centos7-ansible:latest

# add ansible config to user dir
ADD ./ansible/config/ansible.cfg /root/.ansible.cfg

# copy private keys
ADD ./ssh/ansible_ed25519 /root/.ssh/
RUN chmod 700 /root/.ssh
RUN chmod 600 /root/.ssh/*

CMD ["/sbin/init", "-D"]
