# Personal self-hosting (homelab) repo

This project describes my personal self-hosted infrastructure setup, running on a Raspberry Pi 4 board (for now).

This was meant to be just a reminder for me as I can never trust my brain, now I am making it publicly available in case it might help someone out there.

It uses only free and open source software and hardware.

> [!IMPORTANT]
> - The content of this repository is provided "as is", with no guarantee that the information is complete or error-free. Do not just "Copy-Paste", but try to analyze and adapt the content according your use case, especially the docker network (port) and volumes.
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

| Service Name   		|	Port		| Use cases																			| Official Details																									|
|-----------------------|---------------|-----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------	|
| AudioBookShelf		|	80			| Audiobookshelf is a self-hosted audiobook and podcast server.						| [Github](https://github.com/advplyr/audiobookshelf)	[Website](https://www.audiobookshelf.org/)					|
| ActualBudget			|	5006		| Actual is a local-first personal finance tool. 									| [Github](https://github.com/actualbudget/actual)	[Website](https://actualbudget.com/)							|
| CAdvisor				|	8080		| To analyze resource usage and performance characteristics of running containers.	| [Github](https://github.com/google/cadvisor)																		|
| ChangeDetection		|	5000		| Page change monitoring with alerts a breeze.	 									| [Github](https://github.com/dgtlmoon/changedetection.io)	[Website](https://changedetection.io/)					|
| FritzBox-Exporter		|	9787		| This is a prometheus exporter for AVM Fritz! 	 									| [Github](https://github.com/pdreker/fritz_exporter)																|
| Grafana				|	3000		| Just an awesome dashboard.														| [Github](https://github.com/grafana/)	[Website](https://grafana.com/)												|
| HomeAssistant			|	8123		| Open source home automation that puts local control and privacy first.			| [Github](https://github.com/home-assistant/core)	[Website](https://www.home-assistant.io/)						|
| Homer					|	8080		| A simple static HOMepage for your servER to keep your services on hand.			| [Github](https://github.com/bastienwirtz/homer)	[Website](https://homer-demo.netlify.app/)						|
| InfluxDB				|	8086		| An open source time series database for metrics, events, and real-time analytics.	| [Github](https://github.com/influxdata/influxdb)	[Website](https://www.influxdata.com/)							|
| IT-Tools				|	80			| Collection of handy online tools for developers, with great UX.					| [Github](https://github.com/CorentinTh/it-tools)	[Website](https://it-tools.tech/)								|
| Lubelogger			|	8080		| Web-Based Vehicle Maintenance and Fuel Mileage Tracker.							| [Github](https://github.com/hargata/lubelog)	[Website](https://lubelogger.com/)									|
| MySpeed				|	5216		| A speed test analysis software that shows your internet speed						| [Github](https://github.com/gnmyt/myspeed)	[Website](https://myspeed.dev/)										|
| Navidrome				|	4533		| My personal Streaming Service as of using Spotify.								| [Github](https://github.com/navidrome/navidrome/)	[Website](https://www.navidrome.org/)							|
| NextCLoud				|	80			| My private cloud. I hate GoogleDrive, OneDrive.									| [Github](https://github.com/nextcloud)	[Website](https://nextcloud.com/)										|
| Nginx Proxy Manager	|	80, 81, 443	| To easily forward to websites running at home, including free SSL.				| [Github](https://github.com/NginxProxyManager/nginx-proxy-manager)	[Website](https://nginxproxymanager.com/)	|
| Node-Exporter			|	9100		| Exporter for *nix machine metrics													| [Github](https://github.com/prometheus/node_exporter)																|
| Portainer				|	9000		| Making Docker via a Web  UI														| [Github](https://github.com/portainer/portainer)	[Website](https://www.portainer.io/)							|
| Prometheus			|	8080		| The Prometheus monitoring system and time series database.						| [Github](https://github.com/prometheus/prometheus)	[Website](https://prometheus.io/)							|
| Stirling-pdf			|	8080		| Web application that allows you to perform various operations on PDF files		| [Github](https://github.com/Stirling-Tools/Stirling-PDF)	[Website](https://prometheus.io/)						|
| UptimeKuma			|	3001		| An easy-to-use self-hosted monitoring tool.										| [Github](https://github.com/louislam/uptime-kuma)																	|
| Vaultwarden			|	80			| Alternative implementation of the Bitwarden server API.							| [Github](https://github.com/dani-garcia/vaultwarden)																|
| Wiki-JS				|	3000		| A lightweight and powerful wiki app built on NodeJS.								| [Github](https://github.com/Requarks/wiki)	[Website](https://js.wiki/)											|
