### Step 2: Are We Vulnerable? 

**Background:**  Due to the frequency of attacks, your manager needs to be sure that sensitive customer data on their servers is not vulnerable. Since Vandalay uses Nessus vulnerability scanners, you have pulled the last 24 hours of scans to see if there are any critical vulnerabilities.

  - For more information on Nessus, read the following link: https://www.tenable.com/products/nessus

**Task:** Create a report determining how many critical vulnerabilities exist on the customer data server. Then, build an alert to notify your team if a critical vulnerability reappears on this server.

1. Upload the following file from the Nessus vulnerability scan.
   - [Nessus Scan Results](https://vanderbilt.bootcampcontent.com/vanderbilt_coding_bootcamp/vu-virt-cyber-pt-04-2021-u-lol/-/blob/master/2-Homework/18-SIEMs/resources/nessus_logs.csv)

2. Create a report that shows the `count` of critical vulnerabilities from the customer database server.
   - The database server IP is `10.11.36.23`.
   - The field that identifies the level of vulnerabilities is `severity`.

#### source="nessus_logs.csv" host="Nessus_Scans" sourcetype="csv" dest_ip="10.11.36.23" severity=critical

![](https://github.com/kryshael/Week-18-Homework/blob/main/Assets/Severity.png)
      
3. Build an alert that monitors every day to see if this server has any critical vulnerabilities. If a vulnerability exists, have an alert emailed to `soc@vandalay.com`.

![](https://github.com/kryshael/Week-18-Homework/blob/main/Assets/CriticalAlert.png)
