<h1 align="center">Muhammad Aamir Malik</h1>

<p align="center">
  <b>Backend-focused Full Stack Developer</b><br/>
  Node.js · TypeScript · AWS Serverless · React Native
</p>

<p align="center">
  <a href="https://www.muhammadaamirmalik.com/">Portfolio</a> ·
  <a href="https://www.linkedin.com/in/muhammadaamirmalikk">LinkedIn</a> ·
  <a href="mailto:malikaamirdev@gmail.com">Email</a> ·
  <a href="https://www.muhammadaamirmalik.com/assets/Muhammad-Aamir-Malik-CV-Backend.pdf">Backend CV</a> ·
  <a href="https://www.muhammadaamirmalik.com/assets/Muhammad-Aamir-Malik-CV-React-Native.pdf">React Native CV</a>
</p>

---

I build and run Node.js and TypeScript APIs on AWS. I also ship the React Native apps that use those APIs, so I can own a feature from database to screen.

- **4.5+ years** of experience across backends and mobile apps
- **Project Lead** for **Clear Minds Hypnotherapy** at [Algoace](https://algoace.com/), a live wellness app with **100K+ downloads on Google Play** ([Google Play](https://play.google.com/store/apps/details?id=com.clearmindhypnotherapy.app) · [App Store](https://apps.apple.com/app/id1600470480))
- Own its serverless backend: **90+ Lambda functions** across 24 domains and **20 DynamoDB tables**
- Based in Pakistan

## What I do

<table>
<tr>
<td valign="top" width="50%">

**Backend and cloud**

- REST APIs in Node.js and TypeScript with Express.js, Serverless Framework and Middy
- AWS: Lambda, API Gateway, DynamoDB, SQS, S3, Cognito, KMS, CloudFormation, CloudWatch, EventBridge
- Data modelling across DynamoDB, MongoDB and PostgreSQL (Supabase)
- Authentication and access control: Lambda authorizers, JWT verification, role-based access
- Payments: Stripe and RevenueCat webhooks
- Testing and performance: Jest, tinybench, autocannon, GitHub Actions CI

</td>
<td valign="top" width="50%">

**Mobile**

- React Native with TypeScript (CLI, New Architecture, Expo)
- State and data: Zustand, Redux, MMKV, offline caching and downloads
- In-app subscriptions, audio and video playback, Chromecast, push notifications
- Analytics and monitoring: Firebase, Crashlytics, Mixpanel, AppsFlyer
- App Store and Play Store releases

</td>
</tr>
</table>

## Engineering notes

A few problems from the Clear Minds backend and how I solved them.

- **Getting past the CloudFormation 500-resource limit.** The main stack reached 499 resources. I compared nested and sibling stacks, then moved new routes to a separate stack attached to the same API. The app kept one base URL and the production tables were never at risk.
- **Benchmarks that found a real bug.** I benchmarked the API with tinybench and autocannon. The report caught a bug that silently dropped user search results, and database calls that could run in parallel.
- **Tighter API access, with tests.** I hardened access with strict and audit Lambda authorizers and moved them into their own stack. I also added Jest tests for handlers, services and middleware (29 test files).

## Selected work

| Project | What I built | Stack |
|---|---|---|
| **Clear Minds Hypnotherapy**<br/>live audio wellness app | Serverless API with 90+ Lambda functions across 24 domains, 20 DynamoDB tables with secondary indexes and streams, S3 presigned uploads, an SQS queue and 7 scheduled jobs. I also maintain the 40+ screen React Native app with offline downloads, Chromecast and a subscription paywall. | Node.js, TypeScript, Lambda, API Gateway, DynamoDB, React Native |
| **Toggle**<br/>delivery platform for customers, drivers and admins | Most of an Express and MongoDB API on Lambda with 77 endpoints and 16 data models. Cognito JWT auth with three roles, Stripe payments with a signature-verified webhook, driver payouts and a driver document workflow reviewed by admins. | Express.js, MongoDB, Lambda, Cognito, Stripe |
| **Cool Gym Bro**<br/>fitness community | Most of an Express and MongoDB API with 69 endpoints and 12 data models. Gym-ownership claims reviewed by admins, nested comments, voting, reports and notifications using aggregation pipelines and text search. | Express.js, MongoDB, Cognito, KMS |
| **Dreamwhisp**<br/>AI bedtime-story app | Supabase PostgreSQL backend with Edge Functions for story and audio generation, account deletion and a RevenueCat subscription webhook, with tests and GitHub Actions CI. | Supabase, PostgreSQL, Edge Functions |
| **Subscription Planner** | Lambda and DynamoDB API with full Cognito auth flows: sign-up confirmation codes, resend code, forgot and change password, email change and token refresh. | Lambda, DynamoDB, Cognito |
| **FamilyKhata**<br/>personal project | Offline-first family ledger for expenses, loans and savings. SQLite queue and sync engine with conflict detection, a PostgreSQL schema of 28 tables protected by 100 row-level-security policies, and every amount encrypted on the device (XChaCha20-Poly1305). | React Native, Supabase, PostgreSQL, SQLite |
| **Fintech Auth & KYC API**<br/>personal project, in progress | Service for fintech onboarding: OTP and TOTP two-factor login, rate limiting with IP allow and block lists, reCAPTCHA checks, KYC document review and face match. | Node.js, TypeScript, PostgreSQL |
| **MotionFeed**<br/>personal project | TikTok/Reels-style vertical video feed built to hold 60 FPS on mid-range Android, with a live UI/JS FPS monitor. | React Native, Reanimated 4, Gesture Handler, Skia, expo-video |
| **Audventour** | Travel and event app with Stripe payments, Mapbox maps (GPS and offline), push notifications and Google/Apple sign-in. | React Native, Stripe, Mapbox |

The code for these projects lives in private repositories. I am happy to walk through the architecture and the decisions behind it on a call.

## Stack

| Area | Tools |
|---|---|
| Backend and APIs | Node.js, TypeScript, Express.js, REST API design, Serverless Framework, Middy, JSON-schema and request validation |
| Databases | DynamoDB (streams, indexes), MongoDB and Mongoose (aggregation pipelines, text search), PostgreSQL and Supabase (row-level security, triggers, migrations) |
| AWS | Lambda, API Gateway, SQS, S3, Cognito, KMS, CloudFormation, CloudWatch, EventBridge |
| Security and auth | Lambda authorizers, JWT verification, role-based access control, email verification-code flows, encryption of sensitive data |
| Payments | Stripe (payments, signature-verified webhooks, payouts), RevenueCat subscription webhooks |
| Testing and practices | Jest, tinybench, autocannon, code review, GitHub Actions CI, Agile/Scrum |
| Mobile | React Native, TypeScript, Zustand, App Store and Play Store releases |

## Experience

- **Full Stack Developer & Project Lead**, Algoace · Nov 2022 to present
- **React Native Developer**, Softstings, LLC · Feb 2022 to Nov 2022
- **Freelance Full Stack Developer**, Upwork and Fiverr · Feb 2022 to present
- **2nd Place, MERN Stack Hackathon**, Jawan Pakistan · Mar 2022

---

<p align="center">
  Open to backend and full stack roles.
  <a href="mailto:malikaamirdev@gmail.com">malikaamirdev@gmail.com</a> ·
  <a href="https://www.linkedin.com/in/muhammadaamirmalikk">LinkedIn</a>
</p>
