# Chaat & Chill — Restaurant Landing Page
A single-page restaurant website for **Chaat & Chill**, a fictional Indian street food outlet. Built entirely with HTML, CSS, and a bit of JavaScript — no frameworks, no build tools, just clean front-end fundamentals.

## What This Project Is
Chaat & Chill is a fully responsive restaurant landing page that covers everything a real food business website would need — a hero section, an about section, a food category grid, a detailed menu, customer testimonials, a contact form, and a footer. The goal was to make it look and feel like something a real brand would actually put out there.

## Features
- Fixed glassmorphism navbar with a hamburger menu for mobile
- Smooth scroll navigation using jQuery
- Animated hero/showcase section with a background image overlay
- About section with slide-in animation on load
- Food category grid with hover overlays
- Menu section with circular food images and card layout
- Testimonials section with customer review cards
- Contact section with business info panel and a working form layout
- Fully responsive across mobile, tablet, and desktop
- Custom CSS variables for a consistent colour system throughout
  
## Concepts Used
**HTML**
- Semantic sectioning elements (<section>, <nav>, <footer>)
- Anchor-based single-page navigation
- Form structure with labels, inputs, select, and textarea
- External font and icon library integration via CDN
  
**CSS**
- CSS custom properties (:root variables) for a design system
- Flexbox and CSS Grid for layout
- position: fixed navbar with backdrop-filter blur (glassmorphism)
- CSS animations (@keyframes) for slide-in effects on the about section
- Hover transitions on cards, buttons, and overlay effects
- object-fit: cover for consistent image handling
- Media queries for mobile (≤480px, ≤768px), tablet (769px–1024px), and landscape phone
- animation-fill-mode: forwards to lock animation end states
- Responsive typography using rem units with a 62.5% root font-size trick

**JavaScript / jQuery**
- Smooth scroll to anchor sections on nav link click
- Checkbox-based hamburger menu toggle (CSS-driven, JS closes it on link click)

## What I Learnt From This Project
A few things stood out while building this:
- CSS variables are genuinely powerful. Having a single :root block with all the colours and referencing them everywhere made it much easier to stay consistent and tweak the design later without hunting through the whole stylesheet.
- The 62.5% font-size trick changes how you think about rem. Setting html { font-size: 62.5% } means 1rem = 10px, which makes sizing much more intuitive and readable throughout the CSS.
- Glassmorphism is easier than it looks. A translucent background with backdrop-filter: blur() and a subtle box shadow goes a long way for a navbar that feels polished.
- Responsive design needs to be planned, not patched.** I learned that writing mobile queries as an afterthought creates a lot of rewriting. The next project will probably start mobile-first.
- CSS animations with animation-fill-mode: forwards and animation-delay are great for first-load storytelling.** The about section sliding in after the page loads felt like a small thing but made a noticeable difference to how the page felt.
- Small UX details matter. Things like closing the mobile menu automatically when a nav link is clicked, or adding transform: translateY(-3px) on card hover — these aren't features but they make the experience feel finished.

## Project Structure
chaat-and-chill/
├── index.html
├── designpart.css
├── Chaat&Chill.png
├── Chaat and Chill Outlet.png
├── Papdi-chaat.jpg
├── pani-puri.jpg
├── kathi-roll.jpg
├── dahi-bhalla.jpg
├── samosa-chai.jpg
├── sev-puri.jpg
├── ella-olsson-oPBjWBCcAEo-unsplash.jpg
└── (food category images)

## Tech Stack
| Technology     | Purpose                          |
|----------------|----------------------------------|
| HTML5          | Structure and content            |
| CSS3           | Styling, layout, animations      |
| JavaScript     | Smooth scroll, menu toggle       |
| jQuery 3.3.1   | Smooth scroll helper             |
| Font Awesome 6 | Icons (location, phone, socials) |
| Google Fonts   | Poppins typeface                 |

## How to Run
No setup needed. Just clone or download the repo and open `index.html` in any browser. That's it.

## Important Links
- Live Demo — https://chaat-and-chill.vercel.app/
- GitHub Repo — https://github.com/bhargavalok/Chaat-and-Chill.git
- Font Awesome CDN — https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css
- Google Fonts — Poppins** — https://fonts.google.com/specimen/Poppins
- jQuery CDN — https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js

## Notes
- The contact form currently has no backend — form submission does nothing. Can be connected to EmailJS, Formspree, or a custom backend later.
- All food images are either original or sourced responsibly. Swap them out freely for real photography.
- The testimonial section uses static placeholder reviews. These can be made dynamic with a small JSON array and JavaScript if needed later.

Designed & Built by Alok Bhargav — 2026
