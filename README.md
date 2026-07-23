Tavolo 🍅

AI-powered food freshness scanner and zero-waste recipe assistant.

Snap a photo of anything in your fridge or pantry — Tavolo tells you how fresh it is, ranks recipes so the food closest to spoiling gets used first, and connects you to a community of people sharing their own recipes tied to specific ingredients and freshness stages.

"Existing apps track expiry. Tavolo reads freshness."

🌍 The Problem
1.3B tons of food are wasted globally every year — enough to feed 3x the world's undernourished population
Food waste accounts for 8–10% of global greenhouse gas emissions
570M households waste food weekly — households alone account for ~60% of global food waste, more than retail or farms
The root cause: people throw away perfectly edible food because they can't accurately judge freshness

Source: UNEP Food Waste Index · FAO

💡 The Solution

Turn any smartphone camera into a food-freshness expert in three steps:

Snap a photo — point at anything in your fridge or pantry, no barcodes, no typing
AI reads freshness — Vision AI identifies the item and estimates freshness from visual cues (color, texture, ripeness)
Cook it, don't toss it — get recipes ranked by urgency, so what's closest to spoiling comes first
Community Recipe Exchange (in progress)

On top of the AI-ranked recipes, Tavolo lets users submit their own recipes linked to a specific ingredient and freshness stage (e.g. "for very ripe bananas"), with an optional "family recipe" tag. When Tavolo flags your banana as overripe, it can surface a community recipe right alongside the API result — turning food-waste prevention into something people share, not just a solo tool.

⚙️ How It Works
Camera → Vision AI → Detection → Freshness Score → Shelf-Life Estimate → Recipe Recs → Impact Dashboard

A single photo travels through these stages, from lens to plate, in under 1.5 seconds.

🛠️ Tech Stack
Layer	Tech
Frontend	HTML · CSS · JavaScript (+ Bootstrap)
Backend	Flask (Python) · REST API · SQLAlchemy
Vision AI	GPT-4V / Gemini — multimodal inference for item ID + freshness scoring
Recipes	Spoonacular API — ingredient-aware recipe ranking
Database & Auth	PostgreSQL · Flask-Login
Hosting	Render
📊 Impact Tracking

Every scan feeds a personal dashboard showing kg of food saved, CO₂ emissions avoided, and household savings over time — turning food-waste prevention into a measurable, visible habit.

🚀 Getting Started
bash
# Clone the repo
git clone https://github.com/<your-username>/tavolo.git
cd tavolo

# Set up a virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Set environment variables (API keys)
cp .env.example .env
# add your GPT-4V/Gemini and Spoonacular API keys to .env

# Run the app
flask run
🗺️ Roadmap
 Core freshness scanner (photo → AI → freshness score)
 Recipe ranking via Spoonacular
 Community recipe exchange (ingredient + freshness-stage linked submissions)
 Personal CO₂/impact dashboard
 Shared household pantry mode
 Mobile-friendly PWA
👥 Team — SORU Investigation Squad (SIS)
Name	Role
Hemanya D	Team Leader, Fullstack
Lohith S	Backend Developer
Sri Amrita B	Testing & Documentation Lead
Aravindhan K	Frontend & Quality Assurance

Built for PEC Hacks 4.0 — Sustainability track.
