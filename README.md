# Wazuh- All-in-One

![Wazuh](https://wazuh.com/uploads/2022/06/Home.png)

Installation de Wazuh all-in-one sur un serveur Ubuntu 20.04

# Install Ubuntu Server 20.04 LTS 

CPU: 4vCPU
RAM:4 Go
SSD: 128 Go

    apt update && apt upgrade
    systemctl status ufw
    systemctl stop ufw
    curl -sO https://packages.wazuh.com/4.4/wazuh-install.sh
    curl -sO https://packages.wazuh.com/4.4/config.yml

Rajouter l'ip du serveur dans la fichier config.yml

    nano config.yml
  
    bash wazuh-install.sh --generate-config-files
    
    curl -sO https://packages.wazuh.com/4.4/wazuh-install.sh
    
    bash wazuh-install.sh --wazuh-indexer node-1
    
    bash wazuh-install.sh --start-cluster
    
    curl -sO https://packages.wazuh.com/4.4/wazuh-install.sh
    
    bash wazuh-install.sh --wazuh-server wazuh-1
    
    curl -sO https://packages.wazuh.com/4.4/wazuh-install.sh
    
    bash wazuh-install.sh --wazuh-dashboard dashboard

Recuperez le mdp d'Admin dans la fenetre CLI    

Acceder au service : https://ip_du_serveur

  
