# AGRISENSE.AI – Project Documentation

### AI-powered diagnosis and water-first advice for South African agriculture

🌐 Live Website: [AGRISENSE.AI](https://aqua-agro-wise.lovable.app?utm_source=chatgpt.com)

**Version:** 1.1 · May 2026
**Developed by:** Zizipo Malangeni

## Overview

AGRISENSE.AI is a mobile-first AI agriculture platform that helps South African farmers diagnose crop, livestock, soil, and irrigation problems using image analysis and AI-powered advisory tools. The system prioritizes water-saving recommendations to address South Africa’s growing water crisis.

## Core Features

* AI crop, livestock, soil, and irrigation diagnosis
* Water-first recommendations
* AI agricultural advisor chat
* One-tap sample image diagnosis
* Mobile-first responsive interface
* Markdown-based action plans
* South Africa-focused agricultural guidance

## Tech Stack

* **Frontend:** TanStack Start + React 19 + Vite 7
* **Styling:** Tailwind CSS v4
* **Backend:** Lovable Cloud + Supabase Edge Functions
* **AI Model:** Gemini 2.5 Flash via Lovable AI Gateway
* **Markdown Rendering:** react-markdown
* **Notifications:** sonner

## Application Routes

* `/` – Landing page and agriculture insights
* `/diagnose` – Image upload and AI diagnosis
* `/advisor` – AI-powered agriculture chat assistant
* `/insights` – System architecture and technical documentation

## System Architecture

AGRISENSE.AI uses a four-layer architecture:

1. **Client Layer**

   * React-based frontend with file-based routing
   * Mobile-first design for rural accessibility

2. **Edge Layer**

   * Supabase Edge Function acts as a secure proxy
   * Handles validation, CORS, and API protection

3. **AI Layer**

   * Gemini 2.5 Flash multimodal AI model
   * Supports image + text analysis

4. **Data Layer (Planned)**

   * Supabase Postgres + Storage
   * Diagnosis history and farm profiles

## Workflow

1. User uploads an image or selects a sample image
2. Image converts to Base64 format
3. Request sent to `agri-ai` edge function
4. AI generates diagnosis and water-saving recommendations
5. Markdown response rendered in structured format
6. User receives actionable advice

## Water-First Strategy

Every AI response prioritizes water conservation through:

* Drip irrigation recommendations
* Mulching strategies
* Rainwater harvesting advice
* Leak detection guidance
* Drought-resistant crop suggestions
* Load-shedding-aware irrigation timing

## One-Tap Sample Diagnosis (v1.1)

Version 1.1 introduces six preloaded sample diagnoses:

* Sick maize leaf
* Underweight cattle
* Wilted vegetables
* Leaking irrigation system
* Cracked dry soil
* Tomato blight

The sample system reuses the same diagnosis pipeline as manual uploads for consistency and testing reliability.

## Security & Privacy

* API keys stored server-side only
* Edge-function validation and error handling
* No image persistence currently enabled
* Planned Row-Level Security (RLS) with Supabase Auth
* Restricted CORS policies

## Testing & QA

* Mobile responsiveness tested
* All diagnosis routes validated
* Image size and MIME-type validation implemented
* Error handling for 402 and 429 responses
* Sanitized markdown rendering

## Roadmap

### Short-Term

* isiZulu and Sesotho support
* Offline PWA support
* WhatsApp integration

### Mid-Term

* Soil moisture sensor integration
* Weather alerts
* Agricultural co-op partnerships

### Long-Term

* Offline AI vision support
* Finance and insurance integrations

## Conclusion

AGRISENSE.AI demonstrates how AI can support sustainable agriculture in South Africa through intelligent diagnostics, water-first recommendations, and accessible mobile technology. The platform combines multimodal AI, edge computing, and responsive design to deliver practical agricultural support for both smallholder and commercial farmers.

