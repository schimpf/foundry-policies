# Tinag2: Icinga & Nagios Alerts

> Watch Icinga 2 and Nagios problems, acknowledge them and get alerts.

- Android app, Gerrit Schimpf
- Web: https://apps.schimpf.es/tinag2/
- Coming soon to Google Play
- Privacy policy: https://apps.schimpf.es/tinag2/privacy/
- Tools
- Contact: apps@schimpf.es
- DE: https://apps.schimpf.es/tinag2/de/index.md
- ES: https://apps.schimpf.es/tinag2/es/index.md

## About

Tinag2 is an Android client for Icinga 2 and Nagios/Naemon (through Thruk). See what is broken, act on it and get notified, right from your phone.

Connect your own monitoring servers. Add as many as you need; they are fetched in parallel. The app talks only to the servers you enter. There is no account and no developer server.

## Features

### Overview

- Counts of critical, warning and unknown problems and hosts that are down
- A "Needs you now" card for unhandled problems
- Service health bar and a card for each server
- Shows how old the data is, and keeps the last good data when a server cannot be reached

### Problems

- One list sorted by urgency: unhandled first, worst state first, oldest first
- Filters for unhandled, critical, warning and hard states
- Search by text or regular expression
- Services on a host that is down are hidden by default
- Acknowledged and downtime problems are shown muted
- Swipe right to acknowledge, swipe left to recheck. The same actions are available as accessibility actions.
- Detail view with state, check attempts, output, last and next check
- Set a one hour downtime

### Alerts

- Notifies only about new problems or problems that got worse
- The notification is removed when the problem recovers or is handled
- Rules: warnings on or off, skip soft states, skip acknowledged, skip downtime, wait 5 minutes before alerting
- Quiet hours from 22:00 to 07:00, with an option to let critical alerts through
- Separate notification channels for critical and host down, warnings, unknown and connection problems
- Acknowledge directly from the notification

### Widgets

- A counts widget with critical, warning and unknown numbers
- A list widget with the most urgent unhandled problems

### Connection and security

- Icinga 2 REST API and Thruk REST API
- HTTP basic authentication
- Optional pinning of a server's certificate fingerprint, for self-signed servers
- Passwords are encrypted with the Android Keystore
- Plain HTTP is allowed for local networks, and the app warns you when you use it
- No ads, no analytics, no tracking

### Details

Tinag2 needs an Icinga 2 or Thruk server that you can reach from your phone.

- Background sync every 15 minutes, plus pull to refresh
- Light and dark theme that follows the system
- Phone layout with bottom navigation, and a list and detail layout on tablets

## Screenshots

- [Screenshot 1](https://apps.schimpf.es/tinag2/screen-1.png)
- [Screenshot 2](https://apps.schimpf.es/tinag2/screen-2.png)
- [Screenshot 3](https://apps.schimpf.es/tinag2/screen-3.png)
- [Screenshot 4](https://apps.schimpf.es/tinag2/screen-4.png)

## Guides

- [SHA-256 fingerprint of a self-signed Icinga certificate](https://apps.schimpf.es/tinag2/icinga-self-signed-certificate-fingerprint/index.md): How to read the SHA-256 fingerprint of an Icinga 2 or Thruk server certificate with openssl, and how to use it to connect a mobile app safely.
- [Nagios and Icinga soft vs hard states explained](https://apps.schimpf.es/tinag2/nagios-soft-vs-hard-states-explained/index.md): What soft and hard states mean in Nagios and Icinga 2, how check attempts work, and how long a failure takes to become hard. With a worked example.

## Questions and answers

### What does Tinag2 do?

Tinag2 shows the current problems of your Icinga 2 and Nagios/Naemon (through Thruk) servers, sorted by urgency. You can acknowledge a problem, request a recheck, set a one hour downtime and get notified about new or worse problems.

### What does Tinag2 not do?

It checks for new problems every 15 minutes at most, because there is no push service. It supports only Icinga 2 and Thruk, uses only a user name and password (no client certificates), and has no Wear OS app.

### Where does my data stay?

On your phone. The app talks only to the servers you enter, and there is no developer server, no account, no analytics and no ads. Passwords are encrypted with the Android Keystore.

### Do I need to buy anything?

No. The app has no purchases and no ads. You need your own Icinga 2 or Thruk server that your phone can reach.

### Which Android versions does it support?

Android 8.0 or newer.

### Does it work with a self-signed certificate?

Yes. Paste the server certificate's SHA-256 fingerprint into the instance settings and the app accepts that certificate. Without a fingerprint, the certificate must pass the normal Android checks.
