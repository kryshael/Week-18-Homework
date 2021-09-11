### Step 3: Drawing the (base)line

**Background:**  A Vandaly server is also experiencing brute force attacks into their administrator account. Management would like you to set up monitoring to notify the SOC team if a brute force attack occurs again.


**Task:** Analyze administrator logs that document a brute force attack. Then, create a baseline of the ordinary amount of administrator bad logins and determine a threshold to indicate if a brute force attack is occurring.

1. Upload the administrator login logs.
   - [Admin Logins](https://vanderbilt.bootcampcontent.com/vanderbilt_coding_bootcamp/vu-virt-cyber-pt-04-2021-u-lol/-/blob/master/2-Homework/18-SIEMs/resources/Administrator_logs.csv)

2. When did the brute force attack occur?
   - Hints:
     - Look for the `name` field to find failed logins.
     - Note the attack lasted several hours.

#### The attack started on February 21st, 2020 at 2am.

![](https://github.com/kryshael/Week-18-Homework/blob/main/Assets/BruteAttackStart.png)

      
3. Determine a baseline of normal activity and a threshold that would alert if a brute force attack is occurring.

4. Design an alert to check the threshold every hour and email the SOC team at SOC@vandalay.com if triggered. 

Submit the answers to the questions about the brute force timing, baseline and threshold. Additionally, provide a screenshot as proof that the alert has been created.