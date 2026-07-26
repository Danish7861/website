# 🚀 Danish Shahzad AI Portfolio
### AI Engineer • Data Scientist 

> **An AI-powered personal platform engineered to present technical expertise, professional achievements, and interactive portfolio exploration through a production-ready web application.**

This project is more than a traditional portfolio website. It is a complete, end-to-end application designed to help recruiters, hiring managers, clients, and collaborators evaluate technical capabilities through real projects, technical writing, certifications, and an AI assistant capable of answering portfolio-specific questions in real time.

Rather than distributing information across multiple platforms, the application centralises professional experience, project demonstrations, technical articles, certifications, and contact channels into a single, high-performance experience.

Live site: [https://danishshahzadai.com](https://danishshahzadai.com)


<p align="center">

[![Live Website](https://img.shields.io/badge/🌐_Live_Website-danishshahzadai.com-2563EB?style=for-the-badge)](https://danishshahzadai.com)
[![Resume](https://img.shields.io/badge/📄_Resume-Download-success?style=for-the-badge)](https://danishshahzadai.com/cv_datascientist.pdf)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Professional_Profile-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/danishshahzad17)
[![GitHub](https://img.shields.io/badge/GitHub-Danish7861-181717?style=for-the-badge&logo=github)](https://github.com/Danish7861)

</p>


---

## Technology Stack

<p align="center">

![Next.js](https://img.shields.io/badge/Next.js-14-black?logo=next.js&style=for-the-badge)
![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&style=for-the-badge)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&style=for-the-badge)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3-38BDF8?logo=tailwindcss&style=for-the-badge)
![FastAPI](https://img.shields.io/badge/FastAPI-Python-009688?logo=fastapi&style=for-the-badge)
![Gemini_AI](https://img.shields.io/badge/Google-Gemini_AI-4285F4?logo=google&style=for-the-badge)
![Vercel](https://img.shields.io/badge/Deployment-Vercel-black?logo=vercel&style=for-the-badge)

</p>

---
## 1. What This App Is

Danish Shahzad AI Portfolio is a personal portfolio website that presents my work as an Agentic AI Engineer and Data Scientist. It is built to help recruiters, clients, and collaborators quickly understand my background, services, projects, certifications, blog content, and resume in one place.

The real problem it solves is simple: it gives people a fast way to evaluate my skills, review proof of work, and contact me without needing to search through separate profiles, documents, or platforms.

## 2. Who It Is For

- Recruiters who want to review my experience and projects
- Clients looking for AI, automation, analytics, or consulting support
- Students or learners who want to explore my blog and tutorials
- Anyone who wants to contact me directly through the site

## 3. Features

- AI-powered portfolio assistant using Google's Gemini API
- Responsive home page with hero section and portfolio previews
- Responsive user interface built with Next.js and Tailwind CSS
- About, skills, education, experience, projects, services, resume, and contact pages
- Blog system powered by Markdown content files
- Certificates and portfolio evidence showcased across the site
- Contact form for enquiries
- AI chatbot for instant portfolio-related answers
- SEO support with metadata, Open Graph, sitemap, robots, and structured data
- Resume PDF and media assets served from the `public` folder
- Dark/light theme support
- Clean navigation between sections and pages
- Interactive project showcase with detailed project information
- Dynamic Markdown-powered technical blog
- Professional experience and education timeline
- Certification gallery
- Downloadable resume
- Contact form with Resend email integration
- Advanced SEO implementation

## 4. AI Feature

The built-in AI feature is the chatbot on the portfolio site. It answers questions about the portfolio, services, experience, projects, and background by using a system instruction that defines the portfolio context.

### What the chatbot does

- Answers visitor questions about Danish Shahzad’s portfolio
- Helps users find relevant pages, services, and capabilities
- Provides a fast interactive way to learn about the site

### How it works

- The frontend sends the conversation to `app/api/chat/route.ts`
- The backend uses the Gemini API to generate streamed replies
- The assistant is restricted by a portfolio context prompt stored in `lib/portfolioContext`
- The route limits conversation length and response size for stability

### AI instruction / system prompt

The chatbot is guided by a custom portfolio context prompt that tells the model to behave like a concise assistant for this specific website. It is intended to:

- stay focused on the portfolio
- answer accurately from the provided context
- keep replies short and helpful
- avoid inventing unrelated information

## 5. Tools, Services, and Models

- `Next.js` for the frontend framework
- `React` for UI components
- `TypeScript` for type safety
- `Tailwind CSS` for styling
- `FastAPI` for the optional Python backend
- `Resend` for contact form email delivery
- `Gemini API` for the chatbot
- `Vercel` for deployment
- `Markdown` for blog content

## 6. Live Deployment

- Public URL: [https://danishshahzadai.com](https://danishshahzadai.com)

## 7. Screenshots

# Application Preview

### Homepage with hero section
  ![Homepage](./public/screenshots/homepage.png)

### AI Portfolio Assistant (Chatbot open and answering a question)

  ![Chatbot](./public/screenshots/chatbot.png)
  
### Contact Page

  ![Projects](./public/screenshots/projects.png)

## 8. How To Run

### Install dependencies

```bash
npm install
```

### Environment variables

Create `.env.local` from `.env.example` and add:

- `GEMINI_API_KEY`
- `RESEND_API_KEY`
- `CONTACT_EMAIL`
- `RESEND_FROM_EMAIL`

### Start the app

```bash
npm run dev
```

Open `http://localhost:3000` in your browser.

## 9. Optional Python Backend

If you want to run the FastAPI backend used for `/api/py/*` development rewrites:

```bash
pip install -r api/requirements.txt
python -m uvicorn api.index:app --reload
```

The Next.js development setup proxies:

- `/api/py/*`
- `/docs`
- `/openapi.json`

to the local backend on port `8000`.

## 10. Build And Deploy

```bash
npm run build
npm run start
```

For deployment, use the live environment variables on your hosting platform and make sure the public URL matches the one listed above.

## 11. Project Structure

- `app/` - pages, layout, components, and API routes
- `api/` - FastAPI backend
- `content/blog/` - blog markdown files
- `data/` - portfolio content data
- `lib/` - SEO and shared helpers
- `public/` - images, certificates, resume, and static files

## 12. Contact

- Email: `danish.datascientist@gmail.com`
- LinkedIn: `https://linkedin.com/in/danishshahzad17`
- GitHub: `https://github.com/Danish7861`
