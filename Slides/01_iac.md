# Infra as code ?

<!-- .slide: class="page-title" -->




## Définition

TODO



## Approches d'infra as code

- Configuration management, orchestration de déploiement
- Virtualisation, IaaS, Containers
- Software defined \*



## Configuration management

- push/pull
- centralisé / décentralisé
- agent / agentless
- notion de "desired state configuration"
- notion d'idempotence



## Orchestration

- Orchestration de déploiement
  - d'applications
  - d'infrastructures
ex. : Terraform



## IaaS

Déploiement en quelques lignes de code :
 - de machines
 - de réseaux
 - de services d'infrastructure



## Software defined *

Au delà du bullshit : software defined networking

![SDN](ressources/SDN.jpg)



## Software defined networking

![Cisco](ressources/cisco.jpg)

![Cisco CLI](ressources/cisco-cli.jpg)




## Software defined networking

![Cisco web](ressources/cisco-web.jpg)




## Software defined networking

```bash
# Connection issues & priv password
expect {
timeout { send_user "\nTimeout Exceeded - Check Host\n"; exit 1 }
eof { send_user "\nSSH Connection To $hostname Failed\n"; exit 1 }
"*assword:" { send "$password\r" }
}

# Enable password
expect {
default { send_user "\nLogin Failed - Check Password\n"; exit 1 }
"*#" { send "\r" }
"*>" {
send "enable\n"
expect "*assword:"
send "$enablepassword\r"
}
}
```



## Software defined networking

![SDN Architecture](ressources/sdn-architecture.png)



## Software defined networking

![OpenFlow](ressources/openflow.jpg)




## Software defined networking

![ODL](ressources/opendaylight.jpg)




<!-- .slide: class="page-demo" -->
