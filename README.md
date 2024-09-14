# Personal self-hosting (homelab) repo

This project describes my personal self-hosted infrastructure setup, running on a Raspberry Pi 4 board (for now).

This was meant to be just a reminder for me as I can never trust my brain, now I am making it publicly available in case it might help someone out there.

It uses only free and open source software and hardware.

> [!IMPORTANT]
> - The content of this repository is provided "as is", with no guarantee that the information is complete or error-free. Do not just "Copy-Paste" and try to analyze and adapt the content according your use case.
> - The techniques and tools discussed here come with inherent risks.
> - The author and contributors take absolutely no responsibility for possible consequences due to the use of the related software.

## Objective

I started this project in summer 2023 as a **home lab**, for learning purpose and I just want to keep all my data locally located and managed by myself. 

The goal was to have an environment, which is:

- **100% self-hosted** (privacy preserving, full control over data and software)
- **Resource efficient** (The electricity in the country where I live is quite expensive, so I needed to run something resource efficient)
- **Secure** (authentication, SSL/TLS, firewall, ad-blocking, DDOS protection, rate limiting, custom DNS resolver, ...)
- **Lightweight** (runs smoothly with minimal hardware and software requirements)
- **Container-ready** (isolated, portable, scalable applications)
- **Accessible** (some services accessible only locally, some only through VPN, some publicly on the internet)
- **Supervised** (monitoring, alerting, tracking, and backup tools)


## Hardware

Currently all the apps below are running on my [Raspberry Pi 4 Model B](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/)

## Services

I am running and using the following apps. 

| Service Name   	|	Port	| Use cases															| Official Details																									|
|-------------------|-----------|-------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
| Audiobookshelf	|	80		| Audiobookshelf is a self-hosted audiobook and podcast server.		| [Website](https://www.audiobookshelf.org/)	[Github repo](https://github.com/advplyr/audiobookshelf)			|
| ActualBudget		|	5006	| Actual is a local-first personal finance tool. 					| [Website](https://actualbudget.com/)	[Github repo](https://github.com/actualbudget/actual)						|
| Changedetection	|	5000	| Page change monitoring with alerts a breeze.	 					| [Github repo](https://github.com/dgtlmoon/changedetection.io)	[Website](https://changedetection.io/)				|

