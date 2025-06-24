# Task 2 - Analysing a Phishing mail

## 🔍 Objective
  Identify phishing characteristics in a suspicious email sample 

## 🛠 Tools Used
  - Email-header-analyzer  (www.whatismyip.com/email-header-analyzer)
  - Medium Blog (Sample Email)

## 🧪 Steps Performed
  1. Examined the sender's email address
  2. Analysed the email headers
  3. Identified suspicious links
  4. Detailed checking on the language used
  5. Verified spelling/grammer errors

## 📊 Output
  SENDER EMAIL ADDRESS
  - The sender email address (trust.ameribank7.com) is not an official domain of Bank of America. Official domain of Bank of America "bankofamerica.com". 

  EMAIL HEADERS
  - Here the sender mail address and the reply-to are same.Return-Path:(<authenticationmail@trust.ameribank7.com>) exact copy of the sender, as the sender domain is not official the repy-to also re-directing to the attacker. The email source hostname is malicious.

  SUSPICIOUS LINK
  - Malicious link on the body of the email that to reset password using the link given. The link not seem to have the domain name or anything related to the Bank of America, making it suspicious.
  
  LANGUAGE
  - The language used in this context is highly unprofessional. Urges the user to reset their password immediately. There is a clearly visible spelling mistake in the body of the email, such as 'divice' instead of 'device', which further indicates it is not a legitimate message.
    
