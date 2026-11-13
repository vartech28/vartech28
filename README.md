# SV

  I design systems and direct AI agents to build them. Then I own what they ship.

  Right now that's [Crenow](https://crenow.in), a video-editing marketplace that's live and taking real orders. I'm the only technical person there. The engineering
  team is 19 Claude Code subagents, and every change they make goes through a builder, an adversarial reviewer and a browser tester.

  Before this, I spent 10 years in media: 150+ founder interviews as a podcast host, and the storage and network behind a 20-person production team.

  ---

  ## What I'm building

  ### Crenow: a live marketplace

  Brands and creators book vetted freelance video editors. I designed it and directed the whole build, from a Replit prototype to self-hosted production.

  - **19 specialist subagents.** Builder, adversarial code and security reviewer, browser tester and more. Every agent run is logged.
  - **3,000+ automated checks per run** across 13 device profiles, real Android Chrome emulators, iPhone Safari simulation and Lighthouse audits
  - ~5,000 commits across 220+ logged sessions since April 2026
  - Payments in INR (Razorpay) and USD (Stripe) with webhook signature checks, real-time WebSocket chat, and chat moderation that blocks phone, email, card and
  Aadhaar numbers
  - Replit cost about $500 over 3 months before any customer used the platform. The Claude Code workflow cost about $700 over 6 months and built far more.
  - Since going live: 797 editor sign-ups, 7 editors onboarded, 6 orders completed, 2 paying customers

  👉 [crenow.in](https://crenow.in) · [Walkthrough video](https://youtu.be/YY14nlzy-yU) (v1, older than the current platform)

  ### Private infrastructure lab

  6 machines I designed and run: a Proxmox host, 3 Mac minis, a Raspberry Pi and a Windows GPU workstation.

  - 10+ self-hosted services: Gitea, Vaultwarden, n8n, Mattermost, Home Assistant, Frigate NVR
  - An AI operations agent with written rules, access limits and a decision log. 60+ working sessions with it, each closed with a log and a handover.
  - Local document extraction on the GPU workstation: PDFs into structured text with a vision model, fully offline
  - A Mattermost-to-Claude bridge with role-based personas and voice-to-text (5 of 6 phases done)
  - Monitoring: live status dashboard, uptime checks, power-cut detection, Telegram alerts
  - **When things broke:** traced a recurring "host offline" fault to a network-card hardware hang, and recovered corrupted Git repos after a power cut. Both are
  written up as runbooks.
  - A security audit found and closed an unintended cloud data exposure. SSH is key-only, test services are local-only, and credentials live in a vault.

 ### Podcast editing lead-gen engine

  Built for The BOSS Hub and running since September 2026. Multiple n8n workflows, designed by Claude under my direction, that find US podcasts and pitch them
  editing.

  - Scans the Apple Podcasts directory and Google for shows, then finds each show's YouTube channel
  - An AI model scores every show against a lead-scoring method I designed from the business requirements
  - For qualified leads, the AI writes a personalised email from the podcast's latest YouTube episode and sends it through the Gmail API
  - We also sent custom-edited reels to leads
  - Daily Telegram alerts on lead-gen and outreach status

  ### Clauding Hours

  A Mac app I built with Claude Code. It runs alongside your work as a timer and tracks time spent on Claude.

  ---

  ## Stack

  AI agents write the code under my direction. These are the stacks I design for and run.

  **AI & agents**
  `Claude Code` `Multi-agent orchestration` `MCP integrations` `n8n` `Local LLMs (llama.cpp, vision models)`

  **Frontend**
  `React` `TypeScript` `Tailwind CSS` `shadcn/ui` `TanStack Query` `Vite`

  **Backend & data**
  `Node.js` `Express` `PostgreSQL` `Drizzle ORM` `Supabase` `WebSockets`

  **Testing & quality**
  `Playwright` `Vitest` `Lighthouse` `ESLint` `Android emulators` `iOS Simulator`

  **Infrastructure**
  `Proxmox` `Linux (Debian/Ubuntu)` `Podman/Docker` `Tailscale` `Cloudflare Tunnel` `PM2` `Gitea`

  **Storage & networking**
  `TrueNAS` `Unraid` `RAID storage systems` `10G networking` `Managed switches`

  **Payments & APIs**
  `Razorpay` `Stripe` `Cloudflare R2` `Resend` `Zoom API`

  **Google APIs**
  `Gmail API` `Google Drive API` `YouTube API` `Google Calendar API`

  ---

  ## Before AI

  I started The Balls of Steel Show, an entrepreneurship podcast, and hosted 150+ founder interviews. It grew into a podcasting company with a content studio and an
  ad-tech side.
  
  At The BOSS Hub I also ran the tech for about 20 people. Storage went from a single Synology NAS to 2 TrueNAS servers (36 TB each, 10G NICs) shared by 10+ editors.
  When renders slowed down, I traced it to a 1G switch choking the 10G network and swapped it out.
  
  Before that, I was creative director at SV Clicks, a photo and video production house (fashion, product, food, corporate films, animation). Clients over the years
  include Pepsi India, Omaxe and Vahdam Tea.
  
  ---
  
  📍 India (IST) &nbsp;|&nbsp; 🌐 Remote-first &nbsp;|&nbsp; 📧 sarthakv.work@gmail.com 
