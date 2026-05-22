# Metasploit-for-reconnaissance
# Metasploit
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:
 # Checking the Port using ifconfig:
 <img width="617" height="448" alt="592890663-8d8bd114-6fad-4dc0-b72d-c6ac5cde4e36" src="https://github.com/user-attachments/assets/d0b37c85-eb4d-4089-97a9-84e5e2b56ea3" />
# Get into The MsfConsole :
<img width="680" height="576" alt="592890716-19670a90-819f-40d1-a736-d3dd342c1ccc" src="https://github.com/user-attachments/assets/001bd472-15c1-4ba4-b6ca-a644d4a601b1" />
# Using Help Command :
<img width="772" height="602" alt="592890795-cf663e02-96e4-44a3-a08d-246df28f68a0" src="https://github.com/user-attachments/assets/b6ccfced-51b4-467d-b861-6e3d446bbaeb" />

Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.
 # Nmap :
<img width="532" height="145" alt="592890863-d0e1cbe8-2069-41ee-90ee-d9a38edb0e85" src="https://github.com/user-attachments/assets/d150b4e3-0241-4e30-aa52-9c7558efadc8" />
# DB_Nmap :
<img width="640" height="816" alt="592890942-35c94c38-c97b-445b-828c-5aa6c3da0118" src="https://github.com/user-attachments/assets/cc202979-09e6-498f-aa0c-7a93acd349c6" />

Port Scanning:
Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000).
msf >  nmap -sT 192.168.1810/24 -p1-1000  (Replace with appropriate IP Address)
## OUTPUT:

<img width="732" height="397" alt="592891008-3b75de13-4d60-4ae2-94d2-10687dbe4435" src="https://github.com/user-attachments/assets/1ec76dac-3084-4686-92f2-d2c946a58e4b" />

step4:
use the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later.

scan the targets with the command db_nmap as follows.
msf > db_nmap 192.168.181.0/24
## OUTPUT:

<img width="640" height="816" alt="592890942-35c94c38-c97b-445b-828c-5aa6c3da0118" src="https://github.com/user-attachments/assets/4639eea8-20a4-48a6-b2e1-fcdc86c1c7b8" />


Metasploit has a multitude of scanning modules built in. If we open another terminal, we can navigate to Metasploit's auxiliary modules and list all the scanner modules.
cd /usr/share /metasploit-framework/modules/auxiliary
kali > ls -l
## OUTPUT:


<img width="640" height="816" alt="592890942-35c94c38-c97b-445b-828c-5aa6c3da0118" src="https://github.com/user-attachments/assets/53db2bdb-f253-484a-abf8-fefb6b93fba4" />

Search is a powerful command in Metasploit that you can use to find what you want to locate. 
msf >search name:Microsoft type:exploit
## OUTPUT:

<img width="732" height="397" alt="592891008-3b75de13-4d60-4ae2-94d2-10687dbe4435" src="https://github.com/user-attachments/assets/9e0b83b9-559b-487c-a401-7e673745849e" />



The info command provides information regarding a module or platform,

Before beginning, set up the Metasploit database by starting the PostgreSQL server and initialize msfconsole database as follows:
systemctl start postgresql
msfdb init
## OUTPUT:

<img width="732" height="397" alt="592891008-3b75de13-4d60-4ae2-94d2-10687dbe4435" src="https://github.com/user-attachments/assets/3acb8b31-4681-4fff-a8ec-f3dd0c3e2c96" />




## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
