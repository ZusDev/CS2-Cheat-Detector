# CS2 Cheat Detector

### A Counter-Strike 2 Anti-Cheat plugin built on CounterStrikeSharp, designed to protect your server from cheaters in real time.

***Our system goes beyond simple checks – it analyzes player behavior, movement, and aim patterns to catch both rage cheaters and closet players trying to look legit. Unlike traditional plugins that only catch blatant rage hackers, ACD is designed to detect both rage cheaters (spinbot, rapidfire, flickbot) and closet cheaters (silent aim, triggerbot, subtle wallhack). It achieves this by tracking detailed player behavior and applying statistical analysis over time, instead of relying on random guesswork.***

## Requirements

- CounterStrikeSharp
- Metamod

## Features

```
Aimbot & Triggerbot Detection

Detects flickbots, instant flicks, and unnatural trigger timing.


Advanced Aim Pattern Analysis

Identifies semi-rage and rage aimbots.


Silent Aim / Flickbot Defense

Flags unrealistic hit transitions.


Human-Like Smoothness & Velocity Check

Spots cheaters with robotic smoothness or zero reaction time.


Wallhack

Early-stage features for spotting unnatural wall pre-aims and suspicious awareness.


Macro & Spam Protection

Detects bunnyhop scripts, strafe macros, and radio spam.


Discord Webhook Integration

Real-time cheat alerts with evidence and player statistics sent directly to your server’s Discord.

```
## Configuration

```json
{
  "General": {
    "ServerName": "",
    "Webhook": ""
  },
  "Settings": {
    "BanCommand": "css_ban",
    "Duration": 0,
    "SendWebhook": true,
    "Logs": true,
    "AimDataLog": true
  },
  "SpinbotDetection": {
    "Enabled": true,
    "UnnaturalPrecisionThreshold": 180,
    "SuspicionThreshold": 5,
    "BanPlayer": true
  },
  "AimbotDetection": {
    "Enabled": true,
    "MinAimTransitionTime": 120,
    "MaxAngularVelocity": 6.0,
    "SuspicionThreshold": 5,
    "BanPlayer": true
  },
  "Triggerbot": {
    "Enabled": true,
    "MinReactionTime": 120,
    "SuspicionThreshold": 5,
    "BanPlayer": true
  },
  "SilentAimDetection": {
    "Enabled": true,
    "MaxHumanVelocity": 140,
    "SuspicionThreshold": 5,
    "BanPlayer": true
  },
  "WallHackDetection": {
    "Enabled": true,
    "SuspiciousWallbangsThreshold": 6,
    "RDSuspiciousWallbangsThreshold": 3,
    "RDSuspiciousWallshotThreshold": 3,
    "RDSuspiciousAwarenessThreshold": 3,
    "BanPlayer": true
  },
  "Bunnyhop": {
    "Enabled": true,
    "Threshold": 128,
    "BanPlayer": true
  },
  "RapidFire": {
    "Enabled": true,
    "Threshold": 3,
    "BanPlayer": true
  }
}
```

Community Servers – keep casual servers free from closet cheaters.
Competitive Matches – ensure fair play in tournaments.

With CS2 Cheat Detector, you can control your server’s integrity and stay ahead of evolving.

## Official Discord (Updates/Downloads)
<a href="https://discord.gg/d5uvMmUpuE"><img src="./discord.png"></a>



