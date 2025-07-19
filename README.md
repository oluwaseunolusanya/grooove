# Grooove 🎧

**Grooove** is a modern music playlist web app built with **Next.js**. It allows users to search for songs via the Spotify API, build a custom playlist, and save it directly to their Spotify account — all with a fast, responsive interface powered by React and server-side rendering.

---

## 🔑 Key Features

- 🔍 **Spotify Search**: Search for tracks by name, artist, or album
- 🎶 **Real-time Playlist Builder**: Add or remove tracks from a dynamic playlist
- ✅ **Save to Spotify**: Authenticated users can save playlists to their Spotify account
- ⚡ **Next.js**: Fast navigation, server-rendered pages, and API routing
- 💡 **Clean UI**: Built with reusable React components

---

## 📦 Tech Stack

- **Next.js** (React framework)
- **Spotify Web API**
- **CSS Modules** or **Tailwind CSS** (depending on your styling)
- **Node.js** for API routes (via `pages/api`)
- **OAuth 2.0 Authorization** via Spotify

---

## 🚀 Getting Started

### ✅ Prerequisites

- Node.js (v16+ recommended)
- A registered app in the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard)

### ⚙️ Installation

```bash
git clone https://github.com/oluwaseunolusanya/grooove.git
cd grooove
npm install
```

### 🔐 Environment Variables

Create a `.env.local` file in the root of the project:

```env
SPOTIFY_CLIENT_ID=your_spotify_client_id
SPOTIFY_CLIENT_SECRET=your_spotify_client_secret
SPOTIFY_REDIRECT_URI=http://localhost:3000/api/auth/callback
NEXT_PUBLIC_BASE_URL=http://localhost:3000
```

> If using NextAuth.js or a custom auth route, update accordingly.

---

### 🧪 Run the Dev Server

```bash
npm run dev
```

Visit `http://localhost:3000` in your browser.

---

## 🧩 Component Structure

- `pages/` – Next.js routing and static pages
- `components/` – UI components such as:
  - `SearchBar`
  - `SearchResults`
  - `Playlist`
  - `TrackList`
  - `Track`
  - `Button` (e.g., Save to Spotify / Search)

---

## 📁 Project Structure

```
grooove/
├── components/
│   ├── Playlist.js
│   ├── SearchBar.js
│   ├── SearchResults.js
│   ├── Track.js
│   ├── TrackList.js
├── pages/
│   ├── api/
│   │   └── auth.js       # Spotify OAuth handler
│   └── index.js          # Home page
├── styles/
│   └── globals.css
├── .env.local
├── next.config.js
└── README.md
```

---

## 🔁 Commit & Version Control

- Always commit with clear messages:
  ```bash
  git add .
  git commit -m "feat: implement playlist UI"
  git push origin main
  ```

---

## 📝 License

MIT © [Oluwaseun Olusanya](https://github.com/oluwaseunolusanya)

---

## 🤝 Acknowledgements

- [Next.js Documentation](https://nextjs.org/docs)
- [Spotify Web API Docs](https://developer.spotify.com/documentation/web-api/)
- [Tailwind CSS](https://tailwindcss.com) *(if used)*
