# JV Movie - Cyber-Cinematic Streaming Catalog

A modern, responsive, cyber-cinematic movie and TV show catalog platform built as a Single Page Application (SPA) using vanilla HTML, CSS, and JavaScript.

---

## 🛠️ How to Generate & Build This Site (Using AI IDE)

You can generate this streaming website template from scratch using any AI coding assistant (like Antigravity, cursor, etc.) by copying and pasting the prompt below:

### Step 1: Copy and paste this prompt into your AI IDE:

```text
Create a full movie streaming website called "CineStream" using only HTML, CSS, and JavaScript (no backend, no database). Structure it as a single multi-page SPA (Single Page Application) in one index.html file.

DESIGN:
- Dark cinematic theme: background #0a0a0f, accent #e50914 (Netflix-style red), secondary text #a3a3a3
- Font: 'Inter' from Google Fonts for UI, bold display headings
- Fully responsive layout (mobile + desktop)
- Smooth transitions between pages

PAGES & FEATURES:

1. HOME PAGE:
- Top navbar with logo "CineStream", nav links: Home, Movies, TV Series, Search icon
- Hero banner with a featured movie (large backdrop image, title, description, Watch Now + More Info buttons)
- Horizontal scrollable rows: "Trending Now", "Popular Movies", "Top Rated TV Series", "Action Movies", "Korean Drama"
- Each card shows: poster thumbnail, title, rating stars, year
- Hover effect: card lifts with red glow + play icon overlay

2. BROWSE/CATEGORY PAGE:
- Filter bar: All / Movies / TV Series / Genre dropdown (Action, Romance, Drama, Comedy, Horror, Sci-Fi, Korean)
- Grid of movie/show cards (responsive 4-col desktop, 2-col mobile)
- Search bar that filters results live as you type

3. WATCH PAGE (Player):
- Embedded video player using: https://www.2embed.cc/embed/{tmdb_id} for movies and https://www.2embed.cc/embedtv/{tmdb_id}&s=1&e=1 for TV series
- Below player: movie title, rating, year, genre tags, overview/synopsis
- "Related Movies" section showing similar content cards

DATA:
- Fetch movies and TV shows from TMDB API using this base URL: https://api.themoviedb.org/3
- Use API key: (leave a placeholder comment // REPLACE WITH YOUR TMDB API KEY)
- Fetch these endpoints:
  * /trending/all/week for hero + trending
  * /movie/popular for popular movies
  * /tv/popular for popular TV series
  * /movie/top_rated for top rated
  * /discover/movie?with_genres=28 for action
  * /search/multi?query= for search
  * /discover/tv?with_origin_country=KR for Korean drama
- Use poster_path with base: https://image.tmdb.org/t/p/w500
- Use backdrop_path with base: https://image.tmdb.org/t/p/original

NAVIGATION:
- Clicking any movie card goes to Watch Page and passes the TMDB id + media_type
- Back button returns to previous page
- URL hash routing: #home, #browse, #watch?id=XXX&type=movie

CODE STRUCTURE:
- Single index.html file
- All CSS inside <style> tag
- All JS inside <script> tag at bottom
- Use fetch() with async/await for all API calls
- Show loading skeleton cards while fetching
- Error handling: if API fails, show fallback message

Make the website look premium, modern, and cinematic — similar to Netflix or Viu. Include smooth fade-in animations when page loads and when cards appear.
```

### Step 2: Apply Your Free TMDB API Key

⚡ **After your AI IDE generates the codebase**, follow these steps to configure the database content:

1. Register for a free TMDB developer key: Go to **[themoviedb.org/settings/api](https://www.themoviedb.org/settings/api)** and sign up (free and instant).
2. Get your free **API Key (v3 auth)**.
3. Apply it to the code in one of two ways:
   * **Direct UI configuration**: Click the **TMDB API** badge in the header, input the credentials password `Chen@12345678`, paste your key, and save.
   * **In the code file**: Locate the `TMDB_API_KEY` script constant in [index.html](file:///Users/jvs/Portfolio/moviefree/index.html) and replace the placeholder value:
     ```javascript
     const TMDB_API_KEY = 'YOUR_TMDB_API_KEY_HERE';
     ```

---

## ⚡ Key Features of JV Movie Redesign

* **Futuristic Cyber Interface**: Geometric headings (**Righteous**), clean typography (**Poppins**), glassmorphic layout consoles, and neon gradient details (Indigo `#6366f1` to Play Green `#22c55e`).
* **Onboarding Ad-Blocker Alert**: Auto-popups on load recommending browser setups (such as Brave or extensions) to shield video streams from third-party ads.
* **Dynamic API Access Lock**: Security layer (Password: `Chen@12345678`) restricting key settings, which automatically re-locks upon closing.
* **Static SPA Structure**: Zero external build modules, single-file hash routing, and native-feeling CSS page view transitions.

---

## 🚀 How to Run Locally

Run the folder in a local HTTP server container to permit fetch requests:

### Python
```bash
python3 -m http.server 8000
```
Open **[http://localhost:8000](http://localhost:8000)**.

### Node.js (npx)
```bash
npx serve
```

---

## ☁️ Deployment

JV Movie compiles as a static HTML asset and can be hosted for free on:
* **Vercel**
* **Netlify**
* **GitHub Pages**
