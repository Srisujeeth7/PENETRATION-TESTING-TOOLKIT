# PENETRATION-TESTING-TOOLKIT

COMPANY: CODTECH IT SOLUTIONS

NAME: SRI SUJEETH SIRIVELLA

INTERN ID: CT04DN1954

DOMAIN: CYBER SECUTITY & ETHICAL HACKING.

DURATION: 4 WEEEKS

MENTOR: NEELA SANTOSH

TASK DESCRIPTION: FILE INTEGRITY CHECKER

# Objective:

The objective of this project is to design and implement a modular penetration testing toolkit using Python. This toolkit is intended to serve as a basic but functional platform to simulate and analyze vulnerabilities in networks and web systems. By building modules like a Port Scanner and an HTTP Basic Authentication Brute Forcer, the project provides hands-on experience with common attack techniques used by penetration testers and ethical hackers in real-world scenarios.

Penetration testing, also known as ethical hacking, is the process of simulating cyberattacks on systems, networks, or web applications to evaluate their security. The aim is to identify weaknesses before malicious actors can exploit them. Tools used in this domain often include port scanners, brute-force utilities, vulnerability scanners, and enumeration tools. This project emphasizes building such tools from scratch, rather than relying on prebuilt libraries, to deeply understand their inner workings.

## Tools & Technologies Used:

Python 3.13: The main programming language used due to its simplicity, cross-platform support, and rich library ecosystem.

Flask: Used for simulating a secure server that accepts HTTP Basic Authentication.

Socket module: For low-level network programming (TCP port scanning).

Requests module: For web-based HTTP authentication attacks.

Wordlist file: A simple text file simulating a password list for brute-force attacks.

## Toolkit Modules

### 1. Port Scanner

This module performs a TCP port scan on a given IP address (or domain) across a specified range of ports. It attempts to connect to each port using socket programming. If a connection is successful, the port is marked as “open.” Port scanning is one of the most fundamental steps in information gathering for any penetration testing process, as it helps identify open services that may be exploited.

Features:

Customizable port range

Targets both IP and domain names

Returns a list of open ports

Optional: Banner grabbing and multi-threaded scanning (can be added later)

### 2. Brute Forcer (HTTP Basic Auth)

This module performs a password brute-force attack on a website that uses HTTP Basic Authentication. It takes a URL, a known username, and a path to a wordlist file containing passwords. It then iteratively sends HTTP requests using each password until it receives a successful response (status code 200). This simulates how attackers may try to gain unauthorized access using password guessing techniques.

Features:

Uses the Python requests library for clean and simple HTTP requests

Supports custom wordlists

Displays attempted passwords and identifies success

## Testing & Demonstration

To test the toolkit:

A local Flask-based server was created that requires HTTP Basic Auth.

The port scanner was tested on localhost to detect open ports like 8080 where the server was running.

The brute forcer was run against the local server with a wordlist containing the correct password (secret123), successfully cracking the login.

This safe environment allowed ethical testing without harming or scanning unauthorized systems, which is critical in responsible cybersecurity practice.

## Outcomes & Learning

Through this project, key cybersecurity skills were practiced:

Understanding how TCP/IP communication works at the port level.

How HTTP Basic Auth can be attacked if weak credentials are used.

The concept of brute-force attacks and the importance of strong passwords.

Structuring Python code in a modular way for scalability.

Safe testing practices using local servers.

This project lays the groundwork for more advanced modules like:

Directory/file enumeration

SQL injection simulation

Form-based brute-forcing

Password hash cracking

# Conclusion

This Penetration Testing Toolkit serves as an introductory but functional toolset for exploring offensive cybersecurity techniques in a controlled and legal environment. While simple compared to professional tools like Nmap, Hydra, or Burp Suite, building this from scratch provides a solid understanding of the underlying mechanisms that power real-world cybersecurity tools. It’s a valuable step for anyone aspiring to become a penetration tester, ethical hacker, or security analyst.
