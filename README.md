

![](https://github.com/githubissocool/goodbye_goguardian_dns/blob/main/ng.png?raw=true)


# GoodBye GoGuardian (DNS Server)
   (GoGuardian only)
   A hosts list that when added to your DNS server, will completely remove the GoGuardian extension on your Chromebook until reboot (you will have to change DNS back too)
 ---
 ## Status
   🟢 ✅: The host list is working and has been tested to remove goguardian. The hosts list is  working. The hosts lists removes GoGuardian (until reboot) from extensions installed on the  Chromebook making it completely unblocked. 

---
  
## To do:
🟡 Host public dns server. (For now you will have to host your own DNS server and add our list to your server. Then you will have to change the dns servers on the chromebook to use your server. You can also use something like NextDNS)

🟡 Finish the list(s) (still gathering new information and domains from logs)

---

## INFORMATION ABOUT SOME BUT NOT LIMITED TO THESE CONFIRMED DOMAINS AND WHAT THEY DO!!:




1. **beacon-fullpage-predictor.goguardian.com**: This domain is related to GoGuardian Beacon, a student safety solution designed to notify designated staff about online activity that indicates a risk of suicide, self-harm, or possible harm to others. (this basically is used by teachers to tell if youre using websites they dont want you to be on atm like games)

2. **x3-predictor.goguardian.com**: While specific information about this domain is not readily available, it's likely related to GoGuardian's predictive algorithms, given the term "predictor" in the domain name. (this probably means goguardian has some algorithims that are used to determine if it should block this website, for example if you search web proxy goguardian will block it and check if it should be blocked using algorithms. It checks if it should be blocked using its algorithim. Kind of like an extension ad blocker)

3. **panther.goguardian.com**: Specific information about this domain is not readily available, but it's part of the GoGuardian suite, which provides tools for filtering and monitoring online activity, classroom management, and student safety.

4. **ip.goguardian.com**: This domain could be related to GoGuardian DNS, a DNS internet filtering solution that protects devices at the network level.

5. **inquisition.goguardian.com**: The specific function of this domain is not clear from the available information, but it's part of the GoGuardian suite.

6. **countvoncount.goguardian.com**: The specific function of this domain is not clear from the available information, but it's part of the GoGuardian suite.

7. **quiddity.goguardian.com**: The specific function of this domain is not clear from the available information, but it's part of the GoGuardian suite.

8: **blocked.goguardian.com**: The domain is used as a block page. If you see a blocked page even after setting up your own DNS server and adding our list, your doing something wrong.

9. **ext.goguardian.com**: This domain corresponds to the GoGuardian Extension. Here are the main purposes of this domain:
    - Filtering
    - Monitoring
    - Safety

  So when you bootup your chromebook and login to your school account, your chromebook will send a request to this domain. When succesful, the domain will put the GoGuardian Extension on your chromebook.

10. **extapi.goguardian.com**: This domain likely refers to the API (Application Programming Interface) used by GoGuardian. APIs allow different software systems to communicate with each other. In the context of GoGuardian, the API likely facilitates data exchange between the GoGuardian platform and the extensions installed on student devices (explained further in 9).

11. **ws-goguardian.pusher.com**: This domain is related to Pusher, a websocket client used by GoGuardian. It facilitates real-time communication between GoGuardian extensions and the central GoGuardian platform. Essentially, it allows the extensions to send and receive data efficiently

---

## TofSync
Now while you could just desync everything on the Chromebook and restart, that might not work. Unless your assigned a specific Chromebook where you can add accounts. As for me, my school has a login screen, you don't add any accounts you just go straight to the google login screen where you enter your email and password then it logs in, and once you restart, your account is removed, your logged out, everything is gone until you log back on, which this allows other students to use the same Chromebook. Even if you tried Desyncing everything, restarting, and logging back in, everything will still Sync. That is where the TofSync list comes in.

---
So what is TofSync??!?!



TofSync is a new method that prevents Google from syncing anything from your account to the Chromebook, thus effectively removing any other extension blockers such as GoGuardian, Securly, ClassDojo, etc, etc, until you change the DNS back and sync everything. **If you would like to remove TofSync, change the DNS servers and reboot!**



This list by itself, **WILL NOT PREVENT YOU FROM LOGGING INTO YOUR ACCOUNT OR USING YOUR ACCOUNT TO LOG INTO THINGS LIKE CLEVER/CLEVER APPS, GOOGLE CLASSROOM, ETC, ETC**



---
The benefit of TofSync is not only just removing all Extensions, but it will also hide your history. If you have a Chromebook that removes your account completely after restarting, then this will hide your history and once you reboot it can never be recovered or stored since all account data that is stored locally is removed after a reboot. The only way to save the history is if you were to turn off the DNS or remove the hosts list then try syncing again and that will save your history. If you have a Chromebook that allows you to add accounts only and are saved after reboot, then the only way to keep your history hidden is if you keep the DNS on, assuming you cannot clear your history then turn off the DNS, once you turn it on your history is hidden and canoot be synced since your account is not synced, and if you can't clear history then the only way to keep it hidden is using the DNS forever, unless you want it to be synced then all of your history is synced and now they can see it. Let me make this clear that this method, **DOES NOT DELETE YOUR HISTORY**, it only prevents the Chromebook from syncing any history that would be seen if another person were to login to your account and check your history. So if another person lets say, your teacher, were to login to your account from her computer, she wouldn't see any of the history that is locally stored and hidden on the Chromebook, since all data like bookmaarks, shortcuts, and history are saved on your account on Google servers, But if your Chromebook can't sync any of that data from and to those Google Servers, then nothing is saved. And your recent history would only be able to be seen on the Chromebook you were using. If you have a Chromebook you use at school that does not save your account and account data after reboot and instead just removes everything, you wont have to worry about this since it only takes 1 reboot to remove everything and now whatever you just did is forever hidden. So if you were already using the DNS before even logging in, **DO NOT TURN THE DNS OFF OR CHANGE IT** , this will sync everything and stop the exploit from working. **USING THIS METHOD WILL GET RID OF YOUR BOOKMARKS, SHORTCUTS, NEW TAB BACKGROUND IMAGE, PASSWORDS, AND OTHER SETTINGS UNTIL YOU SYNC EVERYTHING**. If you are okay with that like me your good. 👍 


---

## Stable hosts:
Stable hosts are confirmed hosts that are known to be used by GoGuardian. Make a PR if you have new ones.

---

## FYI
I WILL BE UPDATING THE LIST AS FREQUENTLY AS I CAN.
If goguardian realizes these domains are blocked its probably gonna try other domains so i will probably add those if i see it in logs. (if that happens)

This works so far so PLEASE do not try to use scripts or other methods. Scripts are probably patched by now and won't work, you will be wasting your own time. Things like the IncognitoDNS do work till this very day, however this method forces you to use a special unblocked browser and unblocked web proxy while everything else is blocked. The only way you can access websites is through there which isnt as reliable whereas the point is to disable/bypass GoGuardian. This list only disables GoGuardian so everything else works as normal.

## Unstable (suspicous activity) hosts:
So far these domains are cdns only. However I have reason to believe that these may be used since I see these too often. The stable hosts does the job for me so this is probably useless atm. Make a PR if you know more about these domains and if anything should be removed or added.

## For Fun hosts:
So far the only thing this does is potentially disable SafeSearch. I haven't tested it and I am using most of my free time to focus on Stable and Unstable hosts. If you have new domains make a PR.

## Contributing
You can host your own dns server and set it as your dns at school on the Chromebook your using to log domains in the query log so I can add any new ones that popup from your query log (At the moment I do not see any new ones popping up for me) to the list if there is any. You could also use something like NextDNS. Needs to have a query log at the very least. I only want the domain names/ip addresses of the domains, nothing else. Once you have the domains or log make a PR and I will check if there is any new ones and add them.


## Notes for you
1. To add GoGuardian back you will have to change the dns back and reboot. (Changing wifi networks or dns settings and reopening Chrome will do nothing! So you can change wifi networks and GoGuardian will still be removed, until you reboot.)

2. Do not change wifi network right after you login. For this method to take effect you will have to wait until everything loads. Then you can switch wifi networks.

3. If you get "err_connection_reset" even if you disabled goguardian this is likely to do with proxy settings specifically on the browser or the school wifi firewall. I do not know a workaround yet you are gonna have to figure it out yourself. (For me its an issue with a proxy server that was setup by my school at the browser level, it could also be at the network level)
Maybe try blocking the ip of the proxy server with your own dns server.

4. When you login your chromebook might try force a connection to a managed/school wifi even though you were just connected a second ago to the one with custom dns settings. So the second your logged in, (takes 10-15 secs) before everything is loaded/starts loading, turn off wifi, wait till its finished loading as much as it can with wifi off, then turn on wifi and connect to the network with custom dns settings as fast as you can, everything should be unblocked. Enjoy!

5. **DO NOT CHANGE DNS SERVERS** while you are using TofSync, or else everything will sync and the method won't work anymore and you will have to change the DNS Servers again, reboot, and log back in, again.
