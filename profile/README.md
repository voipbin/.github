# VoIPBIN
```
__     __   ___ ____  ____  _        
\ \   / /__|_ _|  _ \| __ )(_)_ __   
 \ \ / / _ \| || |_) |  _ \| | '_ \  
  \ V / (_) | ||  __/| |_) | | | | | 
   \_/ \___/___|_|   |____/|_|_| |_| 
 _   _             ____ ____             ____     __                    _ _
| |_| |__   ___   / ___|  _ \ __ _  __ _/ ___|   / _| ___  _ __    __ _| | |
| __| '_ \ / _ \ | |   | |_) / _` |/ _` \___ \  | |_ / _ \| '__|  / _` | | |
| |_| | | |  __/ | |___|  __/ (_| | (_| |___) | |  _| (_) | |    | (_| | | |
 \__|_| |_|\___|  \____|_|   \__,_|\__,_|____/  |_|  \___/|_|     \__,_|_|_|
```
**VoIPBIN** is a CPaaS (Communications Platform as a Service) designed to simplify and empower voice and messaging solutions for developers, startups, and enterprises alike.

> *"CPaaS for all."*

## 📺 Demo Video
[![Watch the video](./voipbin-demo_flow_build.gif)](https://youtu.be/9VKu_QMFzko)

## 🧩 Live Services
- 🌍 [Project Site](http://voipbin.net/) — Landing page for VoIPbin
- 🔧 [Admin Console](https://admin.voipbin.net/) — Admin console for voipbin(Demo account is ready)
- 📞 [Agent](https://talk.voipbin.net/) — Simple web application demo for agent 
- 🎥 [Meeting](https://meet.voipbin.net/) — Simple web application demo for video/voice conference meeting 

## 📚 Documentation
Detailed documentation is available here:
- 📘 [API Documentation](https://api.voipbin.net/docs/) — Explore and test VoIPbin APIs

## ✨ Features
- **Programmable Voice Flows**: Design advanced call logic using declarative JSON-based Flows with branching, loops, forking, and post-call hooks
- **SMS & Messaging Flows**: Handle incoming and outgoing messages using the same flow engine. Enables surveys, notifications, and chatbot replies.
- **Extension Management**: Register SIP/WebRTC clients, assign extensions, and route calls to the right agent, queue, or flow.
- **Call Queues & Agent Management**: Create call queues with priority rules, agent login/logout, ring strategies, and call wait handling.
- **Outbound Campaigns**: Launch bulk voice or SMS campaigns via API or UI. Campaigns can use flows to automate actions per call/message.
- **Multitenancy & Customer Isolation**: Full tenant separation with isolated configurations, flows, agents, and access control. Designed for SaaS CPaaS scenarios.
- **Conferencing & Moderation Tools**: Host secure, real-time audio conferences with recording, breakout rooms, and moderator roles.
- **Chat & Web Messaging**: Support real-time messaging between customers and agents. Designed for seamless web or mobile integration.
- **AI-Powered Voice**: Integrate chatbot flows that understand user input, trigger smart actions, and provide fallback TTS messaging.
- **Real-time Transcription**: Transcribe speech on the fly or after the call, optionally summarized via AI with customizable flow triggers.
- **Call Recording**: Record conversations, generate transcripts, and summarize content using post-call flow execution.
- **Webhook & HTTP Integration**: Trigger webhooks mid-call or post-call, and dynamically adjust flows based on real-time external responses.
- **Flexible Flow Execution**: Use fork, next_action_id, and conditionals to model real-world conversation logic. Async execution supported.
- **Codec & Media Control**: SRTP, OPUS, PCMU, PCMA support via RTPEngine. Transcoding minimized for low-latency audio.
- **Secure Registration & Authentication**: Digest auth for SIP/WebRTC, token-based auth for API, tenant-based access segregation.
- ... And more and more!

## 📦 Components

VoIPBIN is composed of microservices designed to work together or independently:

* `monorepo`(https://github.com/voipbin/monorepo): Monorepository for the backend services.
* `voipbin-go`(https://github.com/voipbin/voipbin-go): voipbin SDK for golang.

## 🛠️ How to Get Started

> ⚠️ VoIPbin is not a plug-and-play application.
> 
> It's a platform composed of multiple microservices, SIP/media infrastructure (e.g., Asterisk, RTPEngine), Kubernetes-based deployments, and cloud integrations (e.g., Twilio, OpenAI). You don't just "run it" — you assemble and deploy it based on your architecture.

![VoIPBin Architecture](architecture_overview_all.png)

That said, here's how to begin:

### Understand the Architecture

VoIPbin is composed of multiple services that run independently and communicate over HTTP, gRPC, SIP, and WebRTC. You’ll need:

* A Kubernetes environment (we recommend GCP GKE)
* Compute engine with static public IP Address
* A public domain with TLS (e.g., via Cloudflare)
* A media path (RTPEngine or equivalent)
* Optionally, Asterisk instances for call bridging, conferencing, and SIP registration

We recommend reading the platform architecture guide (coming soon) before setup.

## 🤝 Contributing

We welcome contributions! Please open an issue or submit a pull request.

For larger changes, create a discussion or proposal beforehand.

## 📬 Contact
For questions, support, or inquiries, feel free to reach out:

**Email:** sungtae@voipbin.net

## 📜 License
This project is licensed under the MIT License. See the [LICENSE](../LICENSE) for more info.

------
Made with ☎️ by the VoIPBIN team.
