---
title: 'WordCapture'
description: 'Save words while reading or watching, then actually learn them.'
date: 2026-04-25
draft: false
icon: 'globe-2'
tags: ['.NET', 'Kafka', 'MongoDB', 'Kubernetes', 'React Native']
---

I pick up new words everywhere: browsing, reading books, watching something. I wanted every one of
them to go straight into a learning pipeline and be right there on my phone, not lost in a
translator tab.

It's also my own problem solved with my own code and architecture. I'm the user, so I literally
watch my own data flow through the system, feel where it hurts, and fix it.

There's a browser extension for Chrome, Edge and Firefox, and a mobile app that drills words like
Anki, but with typing and saying them out loud. Translations come from DeepL, examples and pictures
are generated, audio is self-hosted TTS.

The backend is a .NET modular monolith with Kafka between modules, MongoDB, Redis and MinIO,
deployed to my own kubeadm cluster on Hetzner via ArgoCD.

It's a private project for now: the app is in a closed beta, the code is not public.
