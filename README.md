# CareerBridge: Your Future Navigator

Build a visually striking, modern frontend for "CareerBridge" — a multi-agent AI 

career platform for students. Use React with Tailwind CSS and Framer Motion for 

animations. This is a demo/mockup for a college project — use mock/placeholder 

data, no real backend needed yet.

## THEME SYSTEM (Important)

- Implement a toggle button (sun/moon icon, top-right of navbar) that switches 

  between LIGHT and DARK themes with a smooth animated transition (fade/crossfade, 

  ~300ms).

- LIGHT THEME: Soft off-white background (#FAFAF7), deep indigo primary (#4F46E5), 

  warm amber accent (#F59E0B), charcoal text (#1F2937). Should feel bright, 

  optimistic, trustworthy.

- DARK THEME: Deep navy/charcoal background (#0F172A), electric violet primary 

  (#818CF8), vibrant amber/gold accent (#FBBF24), off-white text (#F1F5F9). 

  Should feel premium and energetic, not dull.

- Persist theme choice using React state (no localStorage).

- Every component (cards, buttons, nav) must have properly contrasted colors 

  in BOTH themes — test both, don't just invert.

## GLOBAL DESIGN LANGUAGE

- Rounded corners (xl/2xl), soft shadows, glassmorphism accents on cards (subtle 

  backdrop-blur + translucent background)

- Gradient accents on key CTAs (indigo → violet, or amber → orange) 

- Micro-interactions everywhere: buttons scale slightly on hover (scale: 1.05), 

  cards lift with shadow on hover, icons rotate/bounce subtly on hover

- Page transitions: fade + slight slide when switching between agent pages 

  (use Framer Motion's AnimatePresence)

- Smooth scroll-triggered fade-in animations for sections as user scrolls 

  (use Framer Motion's whileInView)

## NAVIGATION

- Top navbar: Logo "CareerBridge", nav links (Home, Features, Dashboard, About), 

  theme toggle button, Login/Signup button

- On Dashboard: a sidebar (collapsible on mobile) with 4 tabs to switch between 

  the agents — clicking a tab animates the content area transition (slide + fade)

## PAGES TO BUILD

### 1. Landing Page

- Hero section: animated gradient text headline "Your career, no connections 

  needed", subheadline about equal opportunity, animated CTA button ("Get Started") 

  with hover glow effect

- Below hero: 4 feature cards in a grid (one per agent below), each with an icon, 

  short title, one-line description, and a "Try it" button — cards should have a 

  hover-lift effect with a subtle gradient border glow

- Stats/impact section with animated counting numbers (e.g., "500+ students helped")

- Footer with simple links

### 2. Dashboard (after login, use dummy student name)

- Welcome banner with student name and a motivational one-liner

- Sidebar navigation to the 4 agent pages below

- Quick-stats cards at top (resume score, career match, scholarships found, jobs matched)

### 3. Agent 1 — Resume Evaluator

- Drag-and-drop file upload box (animated border on drag-hover) for resume PDF

- "Analyze Resume" button with loading animation (pulsing/spinner)

- Results section (mock data): animated circular progress ring showing ATS score 

  (e.g. 72/100), list of improvement suggestions as expandable cards, missing 

  sections shown as flagged chips

### 4. Agent 2 — Career & Exam Counselor

- Multi-step form (animated step indicator at top): Step 1 select stream 

  (Science/Commerce/Arts as selectable cards), Step 2 enter marks, Step 3 

  select interests (multi-select chips)

- "Get Guidance" button

- Results (mock data): 2-3 career path cards that flip or expand on click to 

  reveal reasoning + recommended competitive exams

### 5. Agent 3 — Scholarship & Resource Finder

- Form: income category dropdown, state dropdown, category dropdown 

  (General/OBC/SC/ST), marks input

- "Find Scholarships" button

- Results: scholarship cards (name, amount, eligibility, deadline) in a 

  staggered fade-in list; separate section below for free study resources 

  (YouTube/NPTEL links) grouped by subject, shown as pill tags

### 6. Agent 4 — Job Matcher

- Shows resume-derived skills as animated tag chips at top

- "Find Matching Jobs" button

- Results: job cards (title, company, match % shown as a progress bar, skill 

  gap note) with hover-lift effect

## RESPONSIVENESS

- Fully responsive — sidebar collapses to a bottom nav or hamburger menu on mobile

- Touch-friendly tap targets, since many students will use this on phones

## ICONS

- Use lucide-react icons throughout for consistency

Focus on making this feel premium, trustworthy, and energetic — not like a 

generic dashboard template. This will be demoed live to a college project guide, 

so polish and smoothness of animations matters as much as functionality.

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/4b073045-40a0-4962-9d03-31bf36ddf0e5).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
