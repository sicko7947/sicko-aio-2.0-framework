# SickoAIO Bot Framework (v2.0)

Hi, I’m **Sicko** — many of you might know me from **SickoAIO**, a sneaker/AIO bot I launched back in **2021**. After a successful release of version 1.0, the scene started shifting fast. With my own personal issues and my gradually fading passion for the project, I found myself struggling to keep up, especially with sleeping only 3-4 hours a day and scratch my head off to work around with every akamai update. Additionally, security measures became increasingly sophisticated. As a solo developer, battling against entire CDN security teams became nearly impossible. Eventually, I had to accept that I couldn't maintain the pace required in this rapidly evolving arms race.

But after 4 years, I’ve decided to **open source the entire SickoAIO 2.0 framework**, fully rewritten in **Golang**, with the frontend UI/UX built using **Vue.js**. This is a **high-concurrency**, **scalable** system that may be useful when building performance-critical frameworks — whether for botting, automation, or other use cases.

> ⚠️ **Note:** This project was developed in 2020-2021, and some technical designs or implementations may be **outdated** by today’s standards.

![New Project](https://github.com/user-attachments/assets/464f7536-d337-47e7-aa0e-5f9e7d02d017)

---

## 🧱 Architecture Overview

The framework is modular and split into a few key components:

- [`auth-grpc`](https://github.com/sicko7947/sicko-aio-2.0-auth) – authentication and license verification layer  
- [`server-grpc`](https://github.com/sicko7947/sicko-aio-2.0-server) – core orchestration and for getting cookies or bypassing security measures
- [`client-backend`](https://github.com/sicko7947/sicko-aio-2.0-client) – backend logic for task handling and data flow  
- [`client-frontend`](https://github.com/sicko7947/sicko-aio-2.0-frontend-vue)– UI panel for task management and control  

Each part is designed to be highly concurrent and distributed-friendly.

Technical Design
![image](https://github.com/user-attachments/assets/dc8e7629-5886-4e4f-80a1-e976d93db834)
---

## 🧠 Dev Notes & Insights

Over the years I’ve explored a lot of deep technical areas — from:

- CDN edge caching tricks
- Reverse engineering flows
- [`psychoclient`](https://github.com/sicko7947/psychoclient) Custom HTTP Client with Custom TLS fingerprinting
- Many more...

I plan to **slowly release more repos, writeups, or code samples** on these areas over time.

> ❗ **Important Note:** I will **not** be open sourcing the specific logic I used to tackle Akamai's cookie protection — even if it's outdated — due to **legal and ethical reasons**.

---

## ⚠️ Disclaimer

- This is the **infrastructure behind a bot**, not a ready-to-go bot itself.
- You **will need to test, debug, and adapt** the code to your use case.
- This repo is under Apache2.0 License, you can basically do whatever the fuck you want.
---

