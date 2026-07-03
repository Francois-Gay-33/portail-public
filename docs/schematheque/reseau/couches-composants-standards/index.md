# Couches, composants et standards associés

## Objectif

Ce schéma présente les principales couches du modèle OSI ainsi que les composants, services, protocoles, formats et standards couramment associés.

Il constitue un support pédagogique permettant de :

- Comprendre le rôle de chaque couche.
- Identifier les composants techniques associés.
- Situer les protocoles et standards dans l'architecture.
- Faciliter la lecture des matrices de flux.
- Servir de référentiel commun entre architectes, chefs de projet, exploitants et équipes infrastructure.

---

## Schéma

<img src="schema.svg" alt="Couches, composants et standards

---

## Vue synthétique

| Couche | Rôle principal | Exemples de composants | Protocoles / Standards associés |
|----------|----------|----------|----------|
| 7 - Application | Fournit les services aux applications et utilisateurs | Portails, API, serveurs applicatifs, annuaires | HTTP, HTTPS, DNS, SMTP, LDAP |
| 6 - Présentation | Chiffrement, conversion et encodage des données | PKI, TLS, compression, transformation de formats | TLS, X.509, ASN.1, MIME, UTF-8 |
| 5 - Session | Gestion des dialogues entre applications | SSO, gestion de session, synchronisation | RPC, SMB, NFS, NetBIOS |
| 4 - Transport | Transport fiable ou rapide des données | Load Balancer L4, pare-feu L4 | TCP, UDP, QUIC |
| 3 - Réseau | Routage et adressage logique | Routeur, VPN, pare-feu L3 | IP, ICMP, OSPF, BGP |
| 2 - Liaison de données | Communication locale et adressage MAC | Switch, VLAN, Bridge | Ethernet, Wi-Fi, ARP, STP |
| 1 - Physique | Transmission des signaux | Câbles, fibre, SFP, baie réseau | 1000Base-T, DSL, Bluetooth |

---

## Détail des couches

### Couche 7 – Application

**Rôle :**
Fournir des services réseau directement exploitables par les utilisateurs et les applications.

**Composants courants :**

- Portails et applications
- API REST
- Serveurs applicatifs
- Bases de données
- Messagerie
- Services d'annuaire

**Protocoles courants :**

- HTTP / HTTPS
- DNS
- FTP / SFTP
- SMTP / IMAP / POP3
- SSH
- LDAP
- NTP
- DHCP
- SNMP

---

### Couche 6 – Présentation

**Rôle :**
Assurer la transformation, le chiffrement, l'encodage, la compression et la conversion des données.

**Composants courants :**

- Chiffrement TLS
- PKI
- Conversion JSON/XML
- Compression

**Standards associés :**

- TLS / SSL
- ASN.1
- X.509
- MIME
- JPEG
- ASCII / UTF-8

---

### Couche 5 – Session

**Rôle :**
Établir, maintenir et terminer les sessions de communication entre applications.

**Composants courants :**

- SSO
- Gestion de session
- Contrôle de dialogue
- Synchronisation

**Protocoles associés :**

- NetBIOS
- RPC
- PPTP
- SMB / SMB2
- SQL
- NFS

> Remarque : plusieurs de ces technologies interviennent également sur la couche Application selon les modèles retenus.

---

### Couche 4 – Transport

**Rôle :**
Assurer le transport des données entre deux systèmes, avec contrôle d'erreur et gestion des flux.

**Composants courants :**

- Load Balancer L4
- Pare-feu L4 / NAT
- Contrôle de flux
- Détection d'erreurs

**Protocoles associés :**

- TCP
- UDP
- SCTP
- DCCP
- QUIC

---

### Couche 3 – Réseau

**Rôle :**
Gérer l'adressage logique et le routage des paquets entre réseaux.

**Composants courants :**

- Routeur
- Pare-feu L3
- VPN
- QoS
- Gestion IP

**Protocoles associés :**

- IPv4 / IPv6
- ICMP
- IGMP
- IPSec
- OSPF
- RIP
- BGP
- GRE
- VRRP

---

### Couche 2 – Liaison de données

**Rôle :**
Gérer l'adressage MAC et les communications au sein d'un même segment réseau.

**Composants courants :**

- Switch
- Bridge
- VLAN
- ACL
- Contrôle d'erreurs

**Protocoles associés :**

- Ethernet (802.3)
- Wi-Fi (802.11)
- PPP
- PPPoE
- LACP
- STP / RSTP
- LLDP
- ARP

---

### Couche 1 – Physique

**Rôle :**
Transmettre les bits sur le support physique.

**Composants courants :**

- Câbles cuivre
- Fibre optique
- Connecteurs et modules SFP
- Répéteurs
- Baies réseau
- Alimentation

**Standards associés :**

- 1000Base-T
- 10GBase-SR
- 40GBase-LR
- SONET / SDH
- DSL
- Bluetooth
- NFC
- LoRa
- Z-Wave

---

## Points d'attention pour l'architecture

- Une technologie peut intervenir sur plusieurs couches du modèle OSI.
- Les matrices de flux sont généralement exprimées au niveau **L3/L4** (adresse IP, protocole, port).
- Les couches **L5 à L7** sont davantage liées aux services applicatifs, à la sécurité et aux échanges de données.
- Le modèle **TCP/IP** est plus utilisé opérationnellement que le modèle OSI mais les deux restent complémentaires pour l'analyse et la pédagogie.

---

## Cas d'utilisation

Ce schéma peut être utilisé pour :

- Sensibilisation des chefs de projet.
- Formation aux fondamentaux réseau.
- Construction de matrices de flux.
- Documentation d'architecture.
- Supports de COPIL et ateliers techniques.
- Référentiel de schémathèque.

---

## Références

- Modèle OSI (ISO 7498)
- Architecture TCP/IP
- RFC IETF
- Bonnes pratiques d'architecture réseau

