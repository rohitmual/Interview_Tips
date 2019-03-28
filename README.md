# Interview Tips
This page is a summary of interviews I have been through, covered a decent breadth of roles, got multiple rejects however, learned from each interview, collected constructive feedbacks and went ahead.
Hope these questions/ tips could help you.

Roles which it generally covers are as follows:
- Cybersecurity Intern
- Penetration Testing Intern/ Red Team
- Web App/ Application Security Intern 
- Product Security Intern
- Infrastructure Security Intern

Quick tip:
- Review your resume and ask questions related to it to yourself beforehand
- If you are not aware of any question/concept, don't run around the topic, convey that you could learn it given an environment to work on  
   *You cannot know everything, be humble to accept if you answered something wrong or in need for clarification*
- Prepare a short bio about yourself beforehand to introduce yourself  
- Be sure about your end goal and why infosec?
- Lastly, do ask about feedback at the end of the interview, *why, because:* it helps in knowing and filling the gaps of your current knowledge in infosec

I have tried to jot down all the possible question below which I came across and provided answers for few.
Rest you could google for their specific answers and if you want to dive deep. Apart from that, there are few references in the end do have a look. Those were really helpful.

*Would love to add more question as I move ahead and check my notes, however would appreciate if you could give me a constructive feedback about this by contacting me via jiger13@gmail.com.
If you came across something, which is not covered out here please feel free to share.*

## Common questions

1. Security Triads:

What is CIA?
- Confidentiality
- Integrity
- Availability

What is AAA?
- Authentication
- Authorization
- Accounting

2. Difference between Threat, Vulnerability, Exploits and Risk and how those are related to Assets
- Threat:  
A threat is what we’re trying to protect against
- Vulerability:  
A vulnerability is a weakness or gap in our protection efforts
- Exploit:  
An ability/program (may be a software or social engineering skill) that has been developed to attack an asset by taking advantage of a vulnerability  
- Risk:  
Risk is the intersection of assets, threats, and vulnerabilities
- Asset:  
An asset is what we’re trying to protect

3. What is IAM and why it is been used?   
   IAM is Identity Access Management used to segreagate roles and responsibilities within an organization. It is a critical piece in security. It help in maintaining Access level security and privileges

## Security in general

### Phases of Network Intrusion Attack:
- Reconnaissance/ Information Gathering
- Gaining the needed access
- Maintaining the access
- Covering the tracks (Deleting logs, backdoors and hiding all controls)

## Web Application Security

1. Common Question:
- OWASP Top 10
- What is XSS (Cross-site Scripting)
- How to combat XSS: *Briefly use appropriate input validation*
- Different types of XSS: 
   *Reflected, Stored and DOM-based*
- What are sources and sinks in DOM which could lead to XSS:  
https://www.netsparker.com/blog/web-security/dom-based-cross-site-scripting-vulnerability/
- What is CSRF 
   *This is the sweetest question which every other interviewer would love to ask*  
   *Quick Tip:* Be brief, if asked then only explain the whole story
- How to combat CSRF:  
   Use Anti-CSRF Tokens  
   Use same-origin policy  
- What is HTML/ URL Encoding
- What are types of Injections: *SQL, Command, OS*
- How to combat SQL injections  
   Use paramterized queries and stored procedures

2. There is rare scenario when an interviewer would ask this, I came across this in later stages of few interviews, thought of mentioning:
- What is XXE (XML External Entities)
- What is SSRF (Server Side Request forgery)  
  Could be used to pivot into the internal network
- How to secure 3-tier web architecture
- What is Kerberos
  https://www.varonis.com/blog/kerberos-authentication-explained/
- What is Secret Management and Vaults
  https://www.hashicorp.com/resources/introduction-vault-whiteboard-armon-dadgar

## Network Security
- Difference between Symmetric and Assymetric cryptography
- Difference between Public key cryptography and Assymmtric key cryptography: Both are same *Tricky Question*
- Difference between Encryption, Encoding, Hashing and Obfuscation  
https://danielmiessler.com/study/encoding-encryption-hashing-obfuscation/ 
 - What is Rainbow-table: *Briefly it is a collection of precomputed hashes*
 - How TLS works?  
 *This is an amazing image I stumbled upon, it helped me to understand TLS in layman language*  
 http://i.imgur.com/5T2fJsG.png
 - What is Certificate Signing
 - How Traceroute works
 - How Nmap works
 - What is Certification Authority (CA)
 - What is DMZ and what are the components involved in it
 - What port does ping work over?  
  *A trick question* to be sure, but an important one.   
  Hint: ICMP is a layer 3 protocol (it doesn’t work over a port) A good variation of this question is to ask whether ping uses TCP or UDP. An answer of either is a fail, as those are layer 4 protocols.

## Cloud Security
Would talk in general in terms of AWS, however there are other cloud providers such as Azure, GCP, Digital Ocean, etc..
- General components of AWS:  
   S3, EC2, Buckets, IAM, Cloud trial, Cloud watch
- What is IAM and their components: To be brief IAM is used for Access Management where it used Roles (for temporary access), Policies, Groups and Users for its functioning
- What is EC2: It is an Elastic instance for spinning up a Virtual Machine
- Does EC2 has encrytion: Yes, it does. Amazon EBS encryption offers a simple encryption solution for your EBS volumes without the need to build, maintain, and secure your own key management infrastructure. Amazon EBS encryption uses AWS Key Management Service (AWS KMS) customer master keys (CMKs) when creating encrypted volumes and any snapshots created from them.
More could be found ... below
https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSEncryption.html

## Binary Exploitation

- Tools could be used for debugging a binary:  
   Linux: gdb, radare, clutter (GUI for radare)  
   Windows: IDA, Binary Ninja
- What is Buffer Overflow
- What is Format String Vulnerability
- Difference between Stack and Heap region (Might consider looking into Code, Text and Bss region as well)
- What are Stack Cookies
- What is ASLR and why it is used?
- What is non-executable memory?


## References
OWASP Top 10:  
https://www.owasp.org/images/7/72/OWASP_Top_10-2017_%28en%29.pdf.pdf  
Infosec Interview Questions:  
https://danielmiessler.com/study/infosec_interview_questions  
Top Pentest Questions:  
https://resources.infosecinstitute.com/top-30-penetration-tester-pentester-interview-questions-and-answers-for-2019/#gref  
Python tips:  
https://www.codementor.io/sheena/essential-python-interview-questions-du107ozr6  
AWS User Guide:  
https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html  


