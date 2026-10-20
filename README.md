## DLL Hijacking 🍇
DLL Hijacking project inspired by APT29 GRAPELOADER: https://research.checkpoint.com/2025/apt29-phishing-campaign/

The focus wasn't to recreate GRAPELOADER, but to focus on hijacking a malicious DLL using a trusted binary aspect as well as attempting to write my own simple C2:

I wanted to see if I can use a trusted binary such as powerpnt.exe to load my own malicious DLL, in this case the rust agent. Since for most non-technical users
they're trained to upload malicious exes to something like VirustTotal, in this case they would upload **powerpnt.exe** which is a trusted binary so it will comeback with 0 detections.

However they would likely ignore the malicious DLL and when ran it would connect to the C2 server which is a basic backend written in python with fastapi. 

It's a POC for education and fun.

**For authorized educational and lab research purposes only.**
