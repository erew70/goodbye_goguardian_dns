# GoodBye GoGuardian (DNS Server)

   A hosts list that when added to the DNS used by an ordinary school Chromebook, will              completely remove the GoGuardian extension until reboot (you will have to change DNS again)
 ---
 ## Status
   🟢 ✅: The host list is working and has been tested to remove goguardian. The hosts list is  working. The hosts lists removes GoGuardian (until reboot) from extensions installed on the  Chromebook making it completely unblocked. 

---
  
## To do:
🟡 Host public dns server.
🟡 Finish the list (still gathering new information and domains from logs)

---

## INFORMATION ABOUT SOME BUT NOT LIMITED TO THESE CONFIRMED DOMAINS AND WHAT THEY DO!!:




1. **beacon-fullpage-predictor.goguardian.com**: This domain is related to GoGuardian Beacon, a student safety solution designed to notify designated staff about online activity that indicates a risk of suicide, self-harm, or possible harm to others. (this basically is used by teachers to tell if youre using websites they dont want you to be on atm like games)

2. **x3-predictor.goguardian.com**: While specific information about this domain is not readily available, it's likely related to GoGuardian's predictive algorithms, given the term "predictor" in the domain name. (this shit probably means goguardian is smart and has got some algorithims it uses to tell if ur gonna visit some website or smth like music)

3. **panther.goguardian.com**: Specific information about this domain is not readily available, but it's part of the GoGuardian suite, which provides tools for filtering and monitoring online activity, classroom management, and student safety.

4. **ip.goguardian.com**: This domain could be related to GoGuardian DNS, a DNS internet filtering solution that protects devices at the network level.

5. **inquisition.goguardian.com**: The specific function of this domain is not clear from the available information, but it's part of the GoGuardian suite.

6. **countvoncount.goguardian.com**: The specific function of this domain is not clear from the available information, but it's part of the GoGuardian suite.

7. **quiddity.goguardian.com**: The specific function of this domain is not clear from the available information, but it's part of the GoGuardian suite.

8: **blocked.goguardian.com**: oh wait why is this on here? im pretty sure any student who has suffered the pain of goguardian knows what this is! BOOO! U STINK, FATTY WEBSITE!

9. **ext.goguardian.com**: This domain corresponds to the GoGuardian Extension. Here are the main purposes of this domain:
    - Filtering
    - Monitoring
    - Safety

  So when you bootup your chromebook and login to your school account, your chromebook will send a request to this domain. When succesful, the domain will put the GoGuardian Extension on your chromebook. Meaning that this domain is used specifically to host the extension for schools. e
  Every GoGuardian Extension uses this domain. However, each and every school/district is given a different and unique GoGuardiam Extension. What makes each one stand out and unique is that the Extension ID is different from school to school because the software is paid. Which is why most scripts you find online that uses an extension ID specifically to disable goguardian will most likely not work. Every school/district has their own uniaue GoGuardian Extension ID. My theory on the purpose of a unique ID is to check if it has been paid or pirated, may also be unique to link the extension and admin account to a specific district/school during setup. Pirated GoGuardian Extensions probably serve no use because they are likely linked to a specific district/schoool admin account where all the filtering happems and monitoring with that specific admin account. So in short you have little to no control over a pirated copy at all.

10. **extapi.goguardian.com**: This domain likely refers to the API (Application Programming Interface) used by GoGuardian. APIs allow different software systems to communicate with each other. In the context of GoGuardian, the API likely facilitates data exchange between the GoGuardian platform and the extensions installed on student devices (explained further in 9).

11. **ws-goguardian.pusher.com**: This domain is related to Pusher, a websocket client used by GoGuardian. It facilitates real-time communication between GoGuardian extensions and the central GoGuardian platform. Essentially, it allows the extensions to send and receive data efficiently

---

## Stable hosts:

Stable hosts are confirmed hosts that are known to be used by GoGuardian. Make a PR if you have new ones.

---

## FYI

I WILL BE UPDATING THE LIST AS FREQUENTLY AS I CAN.
If goguardian realizes these domains are blocked its probably gonna try other domains so i will probably add those if i see it in logs. (if that happens)

## Unstable (suspicous activity) hosts:

So far these domains are cdns only. However I have reason to believe that these may be used since I see these too often. The stable hosts does the job for me so this is probably useless atm. Make a PR if you know more about these domains and if anything should be removed or added.

## For Fun hosts:

So far the only thing this does is potentially disable SafeSearch. I haven't tested it and I am using most of my free time to focus on Stable and Unstable hosts. If you have new domains make a PR.

## Contributing
You can host your own dns server and set it as your dns at school on the Chromebook your using to log domains in the query log so I can add any new ones that popup from your query log (At the moment I do not see any new ones popping up for me) to the list if there is any. You could also use something like NextDNS. Needs to have a query log at the very least. I only want the domain names/ip addresses of the domains, nothing else. Once you have the domains or log make a PR and I will check if there is any new ones and add them.
