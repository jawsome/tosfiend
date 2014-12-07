## Mail Policy

**Limits**
  
There is a 500 outgoing email hourly limit per domain. This limit is also applied towards Mailman. If you send over this amount in any hour, most of the e-mails will bounce back with an undeliverable error. If this occurs, it will then take some time for your account to be able to send again so we recommend waiting at least 1 hour after this issue occurs to begin sending email again.

Many of our servers have a limit of 30 POP3/IMAP checks per hour per each user's connecting IP address. If you go over this you're likely to get a wrong password error message or an error stating "login incorrect". If this occurs, please wait an hour and it will automatically unblock you. To prevent this from happening again, please make sure to disable auto checking or at least set it to something higher such as once every 10 minutes.

Any mailing list larger than 5,000 addresses will require a dedicated server or VPS hosting solution from us. Note: Dividing one large list into smaller lists to get below this limit is not allowed.

There is also a limit to the number of Mailman mailing lists permitted as follows (NOTE: This does not apply to other mailing list programs such as PHPList. This only applies to Mailman.)

* Hatchling package: 20 Mailman mailing lists
* Baby package: 25 Mailman mailing lists
* Business package: 50 Mailman mailing lists
* Reseller and Dedicated packages: Unlimited number of Mailman mailing lists

**Mailing Lists Rules**
  
1\. Any time you're sending a message no matter how large your e-mail list is you must throttle it. We recommend you throttle it to at the very least sending 1 email every 8 seconds. (Sending 1 every 8 seconds would send 450 emails within 1 hour, keeping you below the 500 outgoing email limit.) If the mailing list software you're using does not allow you to throttle you must switch to an application or script that will. We recommend PHPList, which can be found in your CPanel, under Quickinstall.

IMPORTANT: If you do not throttle and you try sending 500 emails, the server will try sending all 500 in 1 second which is not possible on our shared servers. This will cause a very high load on the server and the entire server will be sluggish, potentially affecting your sites and service, until this sending process is completed. It is our job to keep the server up and running without being sluggish or experiencing issues. Anyone who causes the server's load to go high will be suspended and the process will be terminated. If you choose not to throttle, you will most likely be suspended for crashing the server.

2\. Any mailing list over 900 email addresses is only allowed to be sent to during off-peak times to prevent high server loads. Off peak times qualify as all day Saturday and Sunday, and 1AM - 8AM Eastern Standard Time, Monday through Friday.

3\. The list must be a Double Opt-In list. This means a user has subscribed for a newsletter or other email marketing messages by explicitly requesting it and confirming the email address to be their own. Confirmation is usually done by responding to a notification/confirmation email sent to the email address the end user specified. The double opt-in method eliminates the chance of abuse where somebody submits someone else's email address without their knowledge and against their will. You will not be permitted to mail any mailing list that you were given or purchased. In doing so, this will also be considered spamming and may result in termination of the offending account.

Email Scripts must be able to handle and document all information from a double opt-in list. This includes recording the sign-up IP address and date/time, double opt-in verification IP address and date/time, processing opt-outs (via web or email), and list removal on bounce backs. All opt-outs or bounce back removals must be handled in a timely manner, and outbound mail must be throttled on shared packages to a maximum of five hundred (500) emails per hour. If your account is found to be using a script that does not meet these requirements, HostGator reserves the right to suspend, terminate, or deactivate your script or account.

4\. Any unsolicited e-mail being sent will result in suspension or termination of the offending account. We take a zero tolerance stance against sending of unsolicited e-mail and other forms of spam.

5\. Any mailling list MUST comply with all guidelines set forth by the United States government. These can be found at: 
  
[http://www.ftc.gov/bcp/edu/pubs/business/ecommerce/bus61.shtm][0] .

6\. No direct SMTP mailers are allowed. An example of this would be a Darkmailer or The Bat!. Any mail should be sent through the local mail server/MTA for further delivery by the server and not done directly by scripts.


[0]: http://www.ftc.gov/bcp/edu/pubs/business/ecommerce/bus61.shtm any and all daemons, such as IRCD.
    3. Run any type of web spider or indexer (including Google Cash / AdSpy) on shared servers.
    4. Run any software that interfaces with an IRC (Internet Relay Chat) network.
    5. Run any bit torrent application, tracker, or client. You may link to legal torrents off-site, but may not host or store them on our shared servers.
    6. Participate in any file-sharing/peer-to-peer activities
    7. Run any gaming servers such as counter-strike, half-life, battlefield1942, etc.
    8. Run cron entries with intervals of less than fifteen (15) minutes.
    9. Run any MySQL queries longer than fifteen (15) seconds. MySQL tables should be indexed appropriately.
    10. Include the local file rather than the URL when using PHP, include functions for including a local file. Instead of including "http://yourdomain.com/include.php"), use "include.php".
    11. Force html to handle server-side code (like php and shtml) to help reduce usage.
    12. Use https protocol unless it is necessary; encrypting and decrypting communications is noticeably more CPU-intensive than unencrypted communications.
  2. **INODES.**
  
The use of more than two hundred and fifty thousand (250,000) inodes on any shared or reseller account may result in a warning, and if no action is taken to reduce the excessive use of inodes, your account may be suspended. If an account exceeds one hundred thousand (100,000) inodes it will be automatically removed from our backup system to avoid over-usage, however, databases will still be backed up as a courtesy in our sole discretion. Every file (i.e. a webpage, image file, email, etc.) on your account uses up one (1) inode.

---

User accounts that constantly create and delete large numbers of files on a regular basis, have hundreds of thousands of files, or cause file system damage may be flagged for review and/or suspension. The primary cause of excessive inodes is typically due to Users leaving their catchall address enabled, but never checking their primary account mailbox. Over time, tens of thousands of messages (or more) build up, eventually pushing the account past an acceptable amount of inodes. To disable your default mailbox, login to cPanel and choose "Mail", then "Default Address", "Set Default Address", and then type in: ":fail: No such user here".
4. **Zero Tolerance Spam Policy**
  1. We take a zero tolerance stance against the sending of unsolicited e-mail, bulk emailing, and spam. "Safe lists," purchased lists, and selling of lists will be treated as spam. We may terminate the account of any User who sends out spam with or without notice. Please read [http://www.hostgator.com/mailpolicy.html][2] for our generalized mail policy. Please read [http://www.hostgator.com/dedicated-mailpolicy.html][3] for our dedicated server mail policy.
  2. Websites advertised via spam (Spamvertised) may not be hosted on our servers. This provision includes, but is not limited to, spam sent via fax, phone, postal mail, email, instant messaging, or usenet/newsgroups. No organization or entity listed in the [ROKSO][4] may be hosted on our servers. Any User account which results in our IP space being blacklisted will be immediately suspended and/or terminated.
  3. HostGator reserves the right to require changes or disable as necessary, any website, account, database, or other component that does not comply with our policies, or to make any such modifications in an emergency that we deem necessary at our sole discretion.
  4. HostGator reserves the right to charge the holder of the account used to send any unsolicited e-mail a cleanup fee or any charges incurred for blacklist removal at our sole discretion.
5. **Defamation Policy.**
  
Websites hosted on HostGator's servers in the U.S. are regulated by U.S. law. Accordingly, pursuant to Section 230(c) of the Communications Decency Act, HostGator's policy is not to remove allegedly defamatory material from websites hosted on our servers unless the material has been found to be defamatory by a court, as evidenced by a court order. As a webhost, HostGator is not a publisher of User content and we are not in a position to investigate the veracity of individual defamation claims. We rely on the legal system and the courts to determine whether or not material is indeed defamatory. In any case in which a court order indicates that material is defamatory, libelous, or slanderous in nature, we will disable access to the material. Similarly, in any case in which a U.S. court has placed an injunction against specified content or material being made available, we will comply and remove or disable access to the material in question.
6. **AUP Violations.**
  1. **Resellers.**
  
If there is a violation of this AUP by one of a reseller's client's account, HostGator will suspend the website in question and will notify the reseller so that the reseller can terminate the account. HostGator may, but is not obligated to, monitor the account or website for any subsequent violations. The occurrence of additional violations may result in the immediate termination of your reseller account.
  2. **Direct customers.**
  
Your Services may be terminated with or without notice upon any violation of this AUP. If applicable, violations will be reported to the appropriate law enforcement agency.
  3. A failure to respond to an email from our abuse department within forty-eight (48) hours, or as otherwise specified in the email, may result in the suspension or termination of your Services. All abuse issues must be dealt with via trouble ticket/email and will receive a response within forty-eight (48) hours.
  4. If you feel you have discovered a violation of our AUP please report it to: [abuse@hostgator.com][0].


[0]: mailto: abuse@hostgator.com
[1]: /copyright "Sample Copyright Infringement"
[2]: /mailpolicy "Mail Policy"
[3]: /dedicated-mailpolicy "Dedicated Mail Policy"
[4]: http://www.spamhaus.org/rokso/ "Register of Known Spam Operations"