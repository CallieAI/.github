🌟 About
Callie AI Caller is an innovative solution for automated service booking designed to help:

😌 Introverts who feel uncomfortable making phone calls
♿ People with disabilities who face communication challenges
⏱️ Busy professionals who value every minute of their time
🛋️ Anyone who prefers convenience and delegating routine tasks

Callie leverages cutting-edge artificial intelligence technology to independently call restaurants, beauty salons, medical clinics, and other establishments, communicate with staff in a natural voice, and make bookings according to your preferences.
✨ Features

🍽️ Restaurant table reservations
💇 Appointments for haircuts and other beauty services
🩺 Medical appointments scheduling
🚗 Taxi or other transportation bookings
🏨 Hotel reservations
🗓️ Manage all your bookings through a convenient mobile app
🔔 Real-time booking status notifications
🌐 Multilingual support

🛠️ Technology

Ultravox — modern AI platform for voice conversation processing
Twilio — reliable API for phone calls
Architecture without STT-LLM-TTS — direct voice processing through a multimodal model
Redis/Database — storage for metadata and booking results
API Gateway — secure entry point for requests
Call Progress Monitor — real-time monitoring of call progress and status

🏗️ Architecture
┌─────────────────┐      ┌───────────────┐      ┌──────────────┐
│  Mobile App     │      │  Callie AI    │      │    Twilio    │
│                 │◄────►│   Backend     │◄────►│   Voice API  │
└─────────────────┘      └───────┬───────┘      └───────┬──────┘
                                 │                      │
                         ┌───────▼───────┐      ┌───────▼──────┐
                         │  Call Progress│      │    TwiML     │
                         │   Monitor     │      │   Executor   │
                         └───────┬───────┘      └───────┬──────┘
                                 │                      │
                         ┌───────▼───────┐      ┌───────▼──────┐
                         │  Ultravox     │◄────►│   Webhook    │
                         │  Client       │      │   Handler    │
                         └───────┬───────┘      └──────────────┘
                                 │                       
                         ┌───────▼───────┐               
                         │  Redis/DB     │               
                         └───────────────┘

