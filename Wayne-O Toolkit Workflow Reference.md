# **Wayne-O Toolkit Workflow Reference**

  

This guide outlines the setup for managing the **Khakis & Kick-Offs** fan toolkit using GitHub, Obsidian, Jekyll, and Carrd.

---

## **🧠 Overview**

  

A hybrid, efficient, Elon-style setup that combines:

- **GitHub** (hosting and version control)
    
- **Jekyll + Just the Docs theme** (docs-style site)
    
- **Obsidian** (markdown-based editing)
    
- **Carrd** (landing page for public access)
    
- **YouTube, X (Threads), Instagram** (content sharing + fan updates)
    

  

This setup will support Wayne-O and his brother’s 12-month journey leading to FIFA World Cup 2026.

---

## **📁 Recommended Website File Structure**

  

A clean, scalable structure that supports current and future needs:

```
/docs
├── index.md                        # Home page (intro, call-to-action, link to toolkit)
├── about.md                        # Project mission, Wayne-O bio, global vision
│
├── planning
│   ├── itinerary.md               # Finalised route overview
│   ├── tickets.md                 # Ticket types, pricing, resale guides
│   ├── flights.md                 # Airlines, hubs, booking tools
│   ├── accommodation.md          # Hotels, Airbnbs, hostels, maps
│   ├── travel-documents.md       # Visas, insurance, passport checklist
│   ├── gear-checklist.md         # Packing lists, essentials, accessories
│   └── budget.md                 # Budget tips, calculators, savings trackers
│
├── host-cities
│   ├── _category_.md             # Overview of host cities
│   ├── los-angeles.md
│   ├── miami.md
│   ├── new-york.md
│   └── toronto.md                # etc.
│
├── stadiums
│   ├── _category_.md             # Stadium overview with seating tips
│   ├── sofi-stadium.md
│   ├── hard-rock-stadium.md
│   └── metlife-stadium.md        # etc.
│
├── matchday
│   ├── checklist.md              # What to bring, day prep
│   ├── safety-tips.md            # Fan safety, police contact, local laws
│   ├── fan-experiences.md        # Cultural tips, chants, dress codes
│   └── flags-chants.md           # Aussie chants, fan-made content
│
├── threads
│   ├── templates
│   │   ├── daily-update-template.md
│   │   └── match-preview-template.md
│   ├── examples
│   │   └── wayneo-opening-game.md
│   └── schedule.md               # Thread posting planner
│
├── youtube
│   ├── shorts-ideas.md
│   ├── video-series.md
│   └── intro-outro-guide.md
│
├── social-media
│   ├── x-threads.md
│   ├── instagram-posts.md
│   └── engagement-strategy.md
│
└── extras
    ├── tools.md                  # Recommended apps, gear, browser tools
    ├── fan-kit.md                # Printable signs, wallpapers, merch links
    └── feedback.md               # Notes from users and collaborators
```

---

## **📄 itinerary.md (Planning > Itinerary)**

```
---
title: Itinerary
nav_order: 1
parent: Planning
---

# ✈️ Wayne-O’s World Cup 2026 Itinerary

Follow the brothers’ journey from Australia to North America as they surf, chant, and footy their way through the FIFA World Cup.

## 🗓️ Timeline

| Date         | Location         | Event/Focus                            |
|--------------|------------------|----------------------------------------|
| June 14      | Los Angeles (LAX)| Arrival, Airbnb setup, sightseeing     |
| June 15–18   | Los Angeles      | Group stage openers, fan events        |
| June 19–22   | Road trip east   | Route 66 vlogging, national parks      |
| June 23–28   | Miami            | Group matches + South American fans    |
| June 29–30   | New York         | Quick hop: culture, night games        |
| July 1–4     | Knockouts phase  | Matchday reactions, hostel hopping     |
| July 5–14    | Follow finals    | Based in Miami, travel for semis/final |
| July 15      | Depart Miami     | 🎥 Recap vlog and trip reflections      |

## 🚘 Route Map (Draft)
- [ ] LA → Vegas → Arizona → Texas → Florida → NYC → Miami
- [ ] Add Google Maps route embed

## 🧳 Packing Philosophy
> “Pack light, shoot often, chant loud.” – Wayne-O

- Clothes: Aussie + football flair
- Media: DJI cam, mic, editing gear
- Flags: Aussie, custom Wayne-O sign
- Safety: First aid, sim cards, backups

## 🗣️ Thread & Video Plan
- Post 1: “He’s baaaaack” – LA arrival
- Post 2: Top 3 chants from first match
- Post 3: Craziest food from the road

> ⚡ This itinerary evolves! Check back for changes as fixtures lock in.
```

---

## **🛠️ Step-by-Step Setup**

  

### **1. ✅ GitHub Repository**

- Create a new public repository on GitHub (e.g. khakis-toolkit).
    
- Enable GitHub Pages under **Settings → Pages**, set source to main and folder to /docs.
    

  

### **2. 🎨 Add Jekyll Template (Just the Docs)**

  

To install Just the Docs into your existing repo:

1. Go to [Just the Docs Template Repo](https://github.com/just-the-docs/just-the-docs-template)
    
2. Click “Use this template” → “Download ZIP” or clone manually
    
3. Copy:
    
    - All files **except** .github/ and README.md into your /docs folder
        
    - pages.yml from .github/workflows into your repo’s .github/workflows/ directory
        
    
4. Edit _config.yml to reflect:
    

```
title: "Khakis & Kick-Offs"
theme: just-the-docs
baseurl: "/khakis-toolkit" # Name of your repo
url: "https://yourusername.github.io"
search_enabled: true
```

---

### **3. 💻 Install GitHub Desktop (macOS)**

- Download: [desktop.github.com](https://desktop.github.com)
    
- Clone your repo locally using GitHub Desktop
    
- This creates a local folder for all files in sync with GitHub
    

  

### **4. ✍️ Edit in Obsidian**

- Open the **local GitHub folder** (e.g. khakis-toolkit) as a Vault in Obsidian
    
- Create and manage all content in Markdown (.md) inside the /docs folder
    
- Use YAML front matter in each page for navigation:
    

```
---
title: Miami
nav_order: 2
parent: City Guides
---
```

### **5. 🧪 Push Changes**

- GitHub Desktop will detect file changes from Obsidian
    
- Use GitHub Desktop to:
    
    - Write a commit message
        
    - Push changes to GitHub
        
    

  

### **6. 🌐 Carrd Landing Page**

- Go to [Carrd](https://carrd.co)
    
- Choose **MAGNA** theme for smooth scroll single-page layout
    
- Use sections for:
    
    - Introduction
        
    - Stadium Guides
        
    - City Guides
        
    - Matchday Checklists
        
    - Wayne-O Threads
        
    
- Link your GitHub Pages site as a “Toolkit” button
    

---

## **🧩 Optional Enhancements**

- Embed Google Maps, flight links, or visa forms in .md pages
    
- Create Thread Templates or daily social copy/paste kits
    
- Schedule Short updates via Threads/X for matchdays
    

---

**You’re now running a fully portable, scalable, fan-first travel toolkit the Elon Musk way — with Aussie charm.** 🦘⚽

# 🌏 Khakis & Kick-Offs – Link Hub

Your ultimate Aussie fan toolkit for the 2026 FIFA World Cup.

---

## 🎒 Main Toolkit

- [🌏 Fan Toolkit Homepage](https://bit.ly/fantoolkit2026)  
  The full planning guide with schedules, packing tips, and more.

- [📅 2026 Match Schedule](/docs/planning/schedule)  
  Key dates across the US, Canada & Mexico.

- [🏟️ Stadium & City Guides](/docs/guides/locations)  
  Local tips, transport, and stadium vibes.

- [🛂 Visa & Travel Checklist](/docs/planning/visas)  
  Entry requirements for Aussies & international fans.

- [🛏️ Accommodation Booking Tips](/docs/planning/stays)  
  From hotels to hostels, road trips and Airbnb hacks.

- [📦 What We Packed (Wayne-O Style)](/docs/planning/packing)  
  Cheeky and practical — what’s in our bags.

---

## 📣 Social Links

- [🎥 Watch Our Journey on YouTube](https://youtube.com/@khakisandkickoffs)  
  Shorts, guides, and Wayne-O antics.

- [📸 Follow on Instagram](https://instagram.com/khakisandkickoffs)

- [🧢 About Wayne-O](/docs/about/wayne-o)  
  Meet the khaki-wearing legend behind the trip.

---

## 🎨 Theme & Styling

- **Primary Color**: `#FFB81C` (Socceroo Gold)
- **Accent / Text**: `#002244` (Navy)
- **Background**: `#F9F9F4` (Sand)
- **Font**: Poppins / Outfit / Rubik

> Used for: Linktree, Carrd, and Just the Docs color scheme