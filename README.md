Phishing – Phishing is a type of social engineering attack where attackers trick people into giving sensitive information, like passwords or credit card numbers, by sending fake emails or creating fake websites.
A phishing email is an email sent by attackers that pretends to be from a trusted source, like a bank, PayPal with the goal of tricking the recipient into revealing sensitive information such as passwords, credit card numbers, or personal details.

In short, a phishing email looks legitimate but is fake and is designed to steal information or install malware.

Step 1: Identification of the Phishing Email

![WhatsApp Image 2025-09-24 at 20 32 46_4ce58720](https://github.com/user-attachments/assets/1086d9be-05c6-4bec-8c5a-3d62b9c18dc1)

I received an email that looked suspicious and appeared to come from a trusted source. Upon reading the email, I noticed several red flags. The email used urgent language, asking the recipient to take immediate action. It contained links that did not clearly match the official website, and there were minor grammatical mistakes in the text. These signs suggested that the email could be a phishing attempt.

Step 2: Email Header Analysis

To verify the legitimacy of the email, I copied the full email headers and analyzed them using online tools, including Google Admin Toolbox – Message Header, PhishTool – Forensic Email Analysis, EasyDMARC – Email Header Analyzer, and LetsPhish – Email Header Analyzer. The results showed that the SPF, DKIM, and DMARC checks all failed, indicating that the email was likely spoofed and did not originate from the legitimate domain. The headers also confirmed the sender, recipient, and date of the email.

<img width="957" height="711" alt="image" src="https://github.com/user-attachments/assets/5693a0a0-da65-4432-beab-6c1f00538088" />

Step 3: IP and URL Analysis

Next, I extracted the sender IP address and all URLs included in the email and checked them using VirusTotal. The sender IP was reported as suspicious, and the URLs were flagged as malicious. This confirmed that both the source of the email and the links within it were unsafe and potentially harmful.

sender ip:198.51.100.22

url:https://example.com/training/paypal-verify?session=TRAINING_TOKEN

Step 4: Website Observation

after clicking the link

![WhatsApp Image 2025-09-24 at 20 32 47_bebbc56b](https://github.com/user-attachments/assets/838aa078-6a09-43b4-bccc-f4b1e60d4c24)

I observed the website linked in the email in a safe environment, such as a sandbox or virtual machine. The website was designed to look exactly like the real service, such as PayPal or Microsoft, in order to trick users into entering their credentials. The email also used urgent language to pressure recipients into clicking the link immediately, which is a common phishing tactic.

submiting the credentials:

![WhatsApp Image 2025-09-24 at 20 32 47_56699311](https://github.com/user-attachments/assets/7003d0f0-ae20-4136-a5a1-944f846405d6)

Step 5: Summary of Findings

Overall, the analysis showed multiple indicators of phishing. The sender address was suspicious and slightly different from the official domain. The email used urgent language and contained minor grammatical errors. The links were misleading and flagged as suspicious by VirusTotal. The email authentication checks, including SPF, DKIM, and DMARC, all failed, further confirming that the email was not legitimate.
