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
  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sample Phishing Email</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      max-width: 700px;
      margin: auto;
      background-color: #f9f9f9;
      padding: 20px;
      color: #333;
    }
    .header {
      font-weight: bold;
      margin-bottom: 10px;
    }
    .section {
      margin-top: 20px;
    }
    .email-body {
      background-color: #fff;
      padding: 20px;
      border-left: 4px solid #d9534f;
      box-shadow: 0 0 8px rgba(0,0,0,0.05);
    }
    .bank-logo {
      width: 180px;
    }
    a {
      color: #007bff;
      text-decoration: none;
      font-weight: bold;
    }
    a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>

  <h2>📧 SAMPLE EMAIL</h2>
  <hr>

  <div class="header">
    <strong>From:</strong> <code>authenticationmail@trust.ameribank7.com</code><br>
    <strong>To:</strong> <code>johnsmith@email.com</code><br>
    <strong>Subject:</strong> <em>A new login to your bank account</em>
  </div>

  <div class="section email-body">
    <img class="bank-logo" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Bank_of_America_logo.svg/320px-Bank_of_America_logo.svg.png" alt="Bank of America Logo">
    <h3>Bank of America</h3>

    <p>Dear account holder,</p>

    <p>There has been a recent login to your bank account from a new device:</p>
    <ul>
      <li><strong>IP address:</strong> <code>192.168.0.1</code></li>
      <li><strong>Location:</strong> Miami, Florida</li>
    </ul>

    <p><strong>4 new transactions have been made with this account since your last login.</strong></p>

    <p><strong>If this was not you, please reset your password immediately with this link:</strong><br>
    👉 <a href="https://trust.ameribank7.com/reset-password" target="_blank">https://trust.ameribank7.com/reset-password</a></p>

    <p>Thank you,<br>
    <strong>Bank America</strong>.</p>
  </div>

</body>
</html>

--------------------------------------------------------------------------------------------


  SENDER EMAIL ADDRESS
  - The sender email address (trust.ameribank7.com) is not an official domain of Bank of America. Official domain of Bank of America "bankofamerica.com". 

  EMAIL HEADERS
  - Here the sender mail address and the reply-to are same.Return-Path:(<authenticationmail@trust.ameribank7.com>) exact copy of the sender, as the sender domain is not official the repy-to also re-directing to the attacker. The email source hostname is malicious.

  SUSPICIOUS LINK
  - Malicious link on the body of the email that to reset password using the link given. The link not seem to have the domain name or anything related to the Bank of America, making it suspicious.
  
  LANGUAGE
  - The language used in this context is highly unprofessional. Urges the user to reset their password immediately. There is a clearly visible spelling mistake in the body of the email, such as 'divice' instead of 'device', which further indicates it is not a legitimate message.
    
