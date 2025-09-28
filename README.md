log4j-shell-poc

A small proof-of-concept project I built to show the impact of the Log4j vulnerability (CVE-2021-44228).

What this repo is

I created this repo to demonstrate a vulnerable Java web application and a proof-of-concept exploit that shows how the vulnerability can be triggered. It’s meant as a learning example so you can see how the issue works and why it's dangerous.

What’s inside

A simple vulnerable web application (Java) that shows how Log4j can be abused.

poc.py — a demonstration script that automates the exploit flow (for study and testing in a safe environment).

A Dockerfile to run the vulnerable app in an isolated container for experimentation.

Example files and small helper scripts used by the demo.

Requirements

I used a few common tools when working with this project:

Python (for the proof-of-concept script)

Docker (to build and run the vulnerable webapp container)

Quick overview — how I set it up

I built the vulnerable web app using the provided Dockerfile and ran it in a contained environment.

I inspected the app and ran the PoC script to see how the vulnerability could be triggered.

The repo includes the pieces needed to reproduce the demo in a lab environment so you can study the flow and the source code.