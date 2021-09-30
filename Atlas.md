# Atlas
This is my writeup for the TryHackMe room [Atlas](https://tryhackme.com/room/atlas) created by [MuirlandOracle](https://tryhackme.com/p/MuirlandOracle).

![image](https://user-images.githubusercontent.com/86648102/135411347-8f13e0b8-c5c2-4758-ba25-e839550dc248.png)

---

## Task 1 Introduction Room Overview and Deploy! 

This is an introductory level room which aims to teach you the very basics of Windows system exploitation, from initial access, through to privilege escalation.

**Answer the questions below**

# Press the Green "Start Machine" button to deploy the machine!

---

## Task 2 Enumeration: Port Scanning 

**Enumeration** is probably the most important thing when comes to solving any challenge.


**Answer the questions below**

### Scan your target IP (10.10.200.252) with Nmap!

Let's add a bit of flavour here, to have a more complex scan with output to a text file for later review:

`sudo nmap -sC -sV -v -oN Atlasnmapscan.txt $ip -p- -Pn`

### With the Nmap default port range, you should find that two ports are open. What port numbers are these?

Reffer to the above **scan** ; the 2 ports are appearing quickly with the verbose output.

### What service does Nmap think is running on the higher of the two ports?

The answer is found in the bottom of the nmap scan.

![image](https://user-images.githubusercontent.com/86648102/135414498-baf3e3fd-48f5-4cfd-b10f-db34df0682c7.png)


### We would usually go on to do a lot more in-depth scanning, but we will leave it at that for this introductory room. We have what we need for the time being.

> Here, it's a reference for the nmap scan switches mentioned above. 

---

## Task 3 Enumeration: Service Enumeration 

