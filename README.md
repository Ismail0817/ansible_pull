# ansible_pull

This repo is to demonstrate ansible pull. It will first download some necessary packages. In this example, cron is mandatory, while others are included just as examples. It will then create a user for ansible with sudo permission. Additionally, it will create a cron job on the machine for the ansible user to check for any changes in the GitHub repo every 10 minutes. If any changes are found, it will implement those changes.

This repo is written for Ubuntu. To run this repo, first install ansible on your machine using the following commands:
```console
sudo apt update
sudo apt install ansible
```

then run the following command:
sudo ansible-pull -U https://github.com/Ismail0817/ansible_pull.git

