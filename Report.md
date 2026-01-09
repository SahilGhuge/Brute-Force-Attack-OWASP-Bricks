# Brute Force Attack Analysis using hydra and burpsuite

## Introduction:
Authentication plays a major role in checking whether the user is valid or not.
Weak Authentication can help the attackers to gain the access on the server or system by using various combinations of passwords and usernames.
This activity is known as "Brute Force Attack".

In this brute force is carried out on the **Owasp Bricks** , which is an intentionally vulnerable web application.
The purpose of this activity is learning and security testing only.


## Objective:
1. To understand brute force attack.
2. To use burpuite and hydra for brute force testing.
3. To study weaknesses in login security.

## Lab Environment:
1. Target : OWASP Bricks
2. Tool Used : Burp suite , Hydra
3. Operating System : Kali Linux
4. Network : Local Lab Environent

All testing was done in a safe and controlled lab setup.

## Brute Force Attack Using Burpsuite:

### Steps:
1. Burp Suite proxy was turned off.
2. The login request was intercerpted.
3. The requet was sent to burp intruder.
4. Username and passwords fields were selected as payloads.
5. Wordlists were loaded.
6. The attack was started.

### Observations: 
1. Many login attempt were allowed.
2. Successfull login was identified by change in response.

## Brute Force Attack Using Hydra:

### Steps:
1. Username and Password wordlists were created.
2. Hydra was used to attack the login form.
3. Multiple login attempts were sent automatically.

### Observations:
1. Credentials were found.

## Result:
Both burp suite and hydra successfully performed brute force attack.

## Mitigations:
1. Limit login attempts.
2. Use strong passwords.
3. Enable multi-factor authentications.

## Conclusions: 
This project shows that weak authentication systems are vulnerable to brute force attacks.  
Using Burp Suite and Hydra in a lab environment helped in understanding how attackers work and how security can be improved.

## Disclaimer
This project is for educational purposes only.  
All testing was done on an intentionally vulnerable application in a controlled lab environment.  
No real systems or accounts were harmed.
