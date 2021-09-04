### Credits --- Anurag Srivastava 

# Red Team Intro 

Pentesting :

- Intial call - Scoping call 
- Scoping e.g - Ip ranges, Objectives 
- Agreement 
- Terms : UAT, staging, 
- Intial recon , mapping of application etc 
- Wireless Hacking, Tailgating, RFID Cloning, Social Engineering, USB baiting


Red teaming :

- Objective based -> goal driven
- Used to test the defense/ detection capabilities
- used to simulate real attack and train the blue team with the detection methods

> Org :  Allooobaba Pvt Ltd.

> Objective : crown jewels : High value system -> HR system, Payroll / Accounts, IT Admin, CEO CSO etc 

www.xyz.com/robots.txt -> 200 /robots.txt IP 

OSINT :

- shodan, censys, virustotal, cert[.]sh, zoomeye
- Linkedin/facebook -> username 
- Existing data leaks 
- recently Aloobaba -> buy -> Pavbhaji 
- Client site attacks - Spear phising, 
- Email -> Macros .docx, .hta

Initial Access  : 

>  Covenent , Empire, PoshC2 - OpenSource C2
- Email Phising - Gophish, kingphish
- Domain reputation, categorization, old/expired domains
- Email Server Setup - SPF record, DKIM record, DMARC record 
- Email Checker - Proofpoint -> DMARC pass 
- 
> EDRs - Carbon black, cylance, symentec, crowdstrike, sophos 


AV Evasion : 

- Signature -> mimikatz.exe -> 
- Sign - \x67\xab\....  aaam != baam XOR -> XOR EBX, EBX -> SUB EBX, EBX -> 


AD :

- Domain -  allobaba.net 
- HVT - Domain Admin -> group Enterprise Admin -> Groups
- HVT -  Domain Controller 
- Attack path -> shivam -> DA 
- Shivam -> DA - no path 
- Shivam -> Member of IT Users group -> List of systems -> Access -> Win67087_hexninja -> Logged in session - nobita -> nobita -> nobita is member of IT Admin -> IT Admin group can access machines in the list -> Machine - Domain Admin group's User Logged in session -> DA group 
- Shivam -> keberoastable users/SPNs -> user killua -> member of DA
- Rubeus -> keberoasting -> 6 Spns hashes -> Hashcat offline dictionary -> 3 crack -> 1 kullua -> DA 
- abc.alloobaba.net -  DA 
- uk.aloobaba.com, us.aloobaba.com child -> Parent -> SID Hijacking / trust exploitation 
- abc.alloobaba.net <-----Bi-directional----> alloobaba.net

SID - S-123-585578- -> shivam
- shivam -> It Users group -> ACL - Generic All -> IT Admin -> DA
- GPOs 


Data Exfilteratio :

- DNS exfilteration 
- ICMP 
- SMB/HTTPS
