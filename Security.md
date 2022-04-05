<!-- 
Dim
S7 App 3
Sécurité des systèmes informatiques
GEI762 
-->

# Email Header

Header is put by MTA for each DNS visited

```
Receved:
    from <AAAA> (<BBBB>[ip])
    ...
    Timestamp
```
### Lookup for
- long Timestamp
- `<BBBB>` is a valid hostname (domain name not a ip)
- `<AAAA>` == `<BBBB>`
- ip reverse lookup give `<AAAA>`

# Phishing
Warnings:
- bad url
- typo
- url shortener

IFrame use to collect info (mask on top of real web page)

# DNS

- SPF: list of valid ip for a domain
- DKIM: public key of MX or MTA that can be validated with server
- DMARC: steps to take if spam

### Fast-flux
change resolution address very quickly

# Cyberattack
### Type:
- social demonstration
- politic ideologie
- financial gain

### Steps:
1. Recon
2. Intrusion
3. Exploitation
4. Erase traces

### Guccifer 2.0 example:
- Actors: APT 28 & 29 (fancy bear & cozy bear) 
- Campagne: Grizzly Steps (spam campagne on political targets)
- Tools: Guccifer 2.0 to communicate between the groups

# STIX
represent a cyberattack in json & graph


# Methbot
bot that click on add for a site to increase click rate for more valuable adds

# Steganography (covert channel)
Hide the existence of a message 

Example:
use header flags of a TCP request

# Tools
## Attack
------
### **Rootkit**
block permission or block visibilitie of files

Levels:

0. not hidden
1. hidden from commands and explorer
2. library modification (.dll)

Example:
- Mebroot

### **Bootkit**
boot malware before os.

**can only be detected by comparing MBR before and after** 

### **Botnet**
Example:
- Torpig

### **Metasploit**
makes use of vulnerability easy to use

### **NMAP**
check open port with `ping` (ICMP) and make fingerprint to find the OS

## Defense
-------
### **Wireshark**
looks at package that passe on the network

### **Dig**
Retrace email ip

### **Iptables** 
rules to dictate the response to specific IP and/or ports

### **HIDS**
make hash of critical files that can be compare in the future to see if something modify the files

Example:
- Tripwire


### **NIDS**
check network patterns to trigger alarm (alarm file) if something suspicious happens.

Example:
- Snort

### **Honeypot**
fake vulnerable machine that has tools to analyse the hacking process
