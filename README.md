# 🎬 Diss-Cuss — Real-Time Movie Discussion Platform

**Diss-Cuss** is a full-stack, production-ready platform designed for film enthusiasts to engage in real-time, Reddit-style threaded discussions around movies and TV shows. It combines a rich UI with deep backend functionality — optimized for scalability, SEO, and modern DevOps.

> 🟢 Live Website: [www.diss-cuss.xyz](https://www.diss-cuss.xyz)  
> 📖 Movie Blogs: [www.diss-cuss.xyz/blogs](https://www.diss-cuss.xyz/blogs)

---

## 🚀 Features

- 🔐 **Authentication** handled via custom backend (Node.js + JWT)
- 🧵 **Threaded Discussions** — Reddit-style nested replies for movies & TV
- 🧠 **AI-Generated Movie Blogs** — 1500-word blog posts via Groq (LLaMA 3)
- 📡 **Real-Time Replies & Likes** — Powered by Socket.io
- 🔎 **Full-Text Search** — Search threads, blogs, and posts using PostgreSQL
- 🖼 **Cloudinary Integration** — For dynamic and fallback image hosting
- 🎞 **TMDB API Integration** — Live metadata for movies and TV series
- ✨ **Rich Metadata & SEO** — Open Graph, Twitter meta, sitemap, and canonical URLs
- 📱 **Mobile-First UI** — Optimized with Tailwind CSS and accessible components
- 🐳 **Containerized Deployment** — NGINX + Docker on a Linux VPS
- ⚙️ **CI/CD Pipeline** — GitHub Actions auto-deploys on `main` pushes

---

## 🗂️ Tech Stack

| Layer           | Tech Used                                                                 |
|------------------|---------------------------------------------------------------------------|
| Frontend         | Next.js (App Router), Tailwind CSS, TypeScript                            |
| Backend          | Node.js + Express, Zod for validation, JWT-based auth                     |
| Database         | PostgreSQL (via Prisma ORM)                                               |
| Auth             | Custom middleware + NextAuth (Google login for client)                    |
| AI Integration   | Groq API (LLaMA 3) for blog generation                                    |
| Image Uploads    | Cloudinary (fallback to Unsplash via keyword matching)                    |
| Real-time        | Socket.io                                                                 |
| External APIs    | TMDB API for live movie/TV data                                           |
| DevOps           | Docker + Nginx proxy + PM2 on VM instance                                 |
| CI/CD            | GitHub Actions (pulls repo → deploys backend via SSH to VM)               |
| Hosting          | Frontend: Vercel | Backend: Custom VM w/ Docker + Nginx                   |

---

## 🧱 Project Structure

```bash
diss-cuss/
├── client/ # Next.js frontend (deployed via Vercel)
│ ├── app/ # App directory (App Router)
│ ├── components/ # Global UI components
│ ├── hooks/ # Custom React hooks
│ ├── utils/ # Utility functions
│ ├── contexts/ # React context providers
│ ├── types/ # TS types
│ └── actions/ # Client-side business logic
├── server/ # Node.js backend (Express)
│ ├── routes/ # REST endpoints (auth, threads, blogs)
│ ├── controllers/ # Route handlers
│ ├── middleware/ # JWT auth, error handlers
│ ├── prisma/ # DB schema and queries
│ └── utils/ # Logging, config, services (Groq, Cloudinary, etc.)
├── docker/ # Dockerfile and nginx.conf
└── .github/workflows/ # GitHub Actions for CI/CD
```

---
## 📸 Screenshots
- Home Page
  ![image](https://github.com/user-attachments/assets/debc3852-1892-451b-a08b-898e9c0af9be)

  
- List Page
  ![image](https://github.com/user-attachments/assets/9a31b10b-dbf8-4f29-9471-cc245d5c02cc)

  
- Search Page
  ![image](https://github.com/user-attachments/assets/63cd311f-5f0c-454d-9bea-e26b40bb7af1)

  
- Blogs Page
  ![image](https://github.com/user-attachments/assets/19cc903c-b3bf-4198-9467-68e2d80b3b23)

  
- Create Blog
  ![image](https://github.com/user-attachments/assets/073aa36c-6184-4f03-9fb2-0b09922fc957)

  
- Blog Page
  ![image](https://github.com/user-attachments/assets/0f133199-f973-4242-8f31-0b44453e6fea)

  
----

## 🧑‍💻 Author

Nitin
✉️ [mk3529895@gmail.com](mailto:mk3529895@gmail.com)
🌐 [www.diss-cuss.xyz](https://www.diss-cuss.xyz)

## 📄 License

This is a private project licensed under the MIT License. Contact [mk3529895@gmail.com](mailto:mk3529895@gmail.com) for inquiries.
