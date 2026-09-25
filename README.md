# Amazon Fire TV: Emotion-Aware Personalization 🎬

> **Amazon HackOn 5.0 | Product Innovation Case Study | June 2025**

**Team HeYou — Hemakshi Kumar & Youkta Mandavkar**

🔗 [Amazon HackOn 5.0](https://tinyurl.com/az-hack-on)

---

## 📌 Overview

Streaming platforms offer thousands of titles, but more choice often creates **decision fatigue rather than better discovery**.

For Amazon Fire TV, we identified three key user pain points:

- 🎭 **Content overload** — recommendations can feel repetitive or impersonal.
- 🧠 **Lack of emotional context** — users often choose content based on their current mood rather than genre alone.
- 👥 **Fragmented social discovery** — viewers lack lightweight ways to discover and share content through people they know.

We proposed an **AI-driven, emotion-aware personalisation layer for Fire TV** that combines mood, viewing history, time-of-day behaviour, and social context to make content discovery more relevant.

---

## 💡 Product Vision

### **"You set the vibe. Fire TV finds what fits."**

The solution consists of two complementary experiences:

### 1. 🎭 Emotion-Aware Personalization

A mood-aware recommendation system that combines:

- **User-selected mood**
- **Viewing history**
- **Time-of-day viewing patterns**

to dynamically personalise content recommendations.

Instead of asking:

> *"What genre do you want?"*

Fire TV can understand:

> *"What do you feel like watching right now?"*

---

### 2. 🤝 "Unify" — Social Watch Discovery

A social discovery layer designed for shared-device households and friends.

**Unify** enables:

- Profile blending for common interests
- Joint recommendations
- Synced watchlists
- Friend/activity-based content cues
- Co-watching prompts

The experience is designed to remain **optional and low-friction**, without requiring synchronous viewing or chat.

---

## 👥 Target Users

### Gen Z & Young Adults

- Prefer mood-based discovery over browsing by genre
- Want instant, curated recommendations
- Seek social discovery without necessarily watching simultaneously

### Shared-Device Households

- Multiple users maintain separate profiles
- Want personalisation without completely mixing preferences
- Benefit from intelligent overlap between viewing interests

These user needs were translated directly into product features through a **working-backwards approach**. :contentReference[oaicite:1]{index=1}

---

## 🔍 User Need → Product Response

| User Need | Product Response |
|---|---|
| Mood-based discovery | Mood input drives recommendations |
| Content fatigue | Fresh and diverse suggestions |
| Socially relevant discovery | **Unify** surfaces friend/activity-based cues |
| Low-friction interaction | Remote-friendly, button-based interaction |
| Multiple viewers | Profile blending + joint recommendations |

:contentReference[oaicite:2]{index=2}

---

## 🧠 Recommendation Engine

The proposed recommendation pipeline follows:

```text
                    ┌──────────────────┐
                    │   User Signals   │
                    └────────┬─────────┘
                             │
              ┌──────────────┼──────────────┐
              ↓              ↓              ↓
        Viewing History   User Mood    Time of Day
              │              │              │
              └──────────────┼──────────────┘
                             ↓
                  ┌────────────────────┐
                  │ Recommendation     │
                  │ Engine             │
                  └─────────┬──────────┘
                            ↓
                  Ranked Recommendations
                            ↓
                    Fire TV Interface
                            ↓
                     User Feedback
                            │
                            └──────→ Model
                                    Improvement
