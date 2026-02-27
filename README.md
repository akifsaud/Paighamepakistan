# Paigham-e-Pakistan — Official Website

## The World's First Revolutionary Human Rights & Peace Initiative

A production-ready, multi-page website for the Paigham-e-Pakistan initiative — breaking the cycle of crime through education by providing comprehensive educational support and scholarships for children of convicted prisoners in Sindh's jails.

---

## 🌐 Site Structure & Pages

| # | Page | File | Description |
|---|------|------|-------------|
| 1 | **Home** | `index.html` | Hero with animated stats, focus areas, about preview, leader quotes, news updates, partners, CTA |
| 2 | **About Us** | `about.html` | Chairman's message, vision & mission, team profiles, FAQ accordion, partners |
| 3 | **Messages** | `messages.html` | Quaid-e-Azam quote, Field Marshal Asim Munir message, government officials messages |
| 4 | **Our Initiative** | `initiative.html` | Scholarship program details, rehabilitation framework, peacebuilding efforts, implementation strategy, stats bar |
| 5 | **Events & Activities** | `events.html` | Launching ceremony, workshops, 4-phase scholarship distribution timeline |
| 6 | **Impact & Outcomes** | `impact.html` | Animated metrics, success stories with quotes, long-term vision (6 goals) |
| 7 | **Media Center** | `media.html` | Press releases, photo gallery (8 images), video gallery, media kit |
| 8 | **Resources** | `resources.html` | Tabbed interface: Publications, Educational Materials, Legislation, International Standards |
| 9 | **Contact & Collaboration** | `contact.html` | Contact form with validation and API storage, contact info, 4 collaboration types, social media |

---

## 🖼️ Image Assets — Extracted & Placed Per Page

### Downloaded Images (11 files in `images/` directory)

| Image File | Size | Used On | Content Description |
|-----------|------|---------|---------------------|
| `children-education.jpg` | 321 KB | Home (hero), Initiative (scholarship), Impact (hero), Media (gallery, press) | Children receiving educational support |
| `children-classroom.jpg` | 245 KB | Home (news), Initiative (hero bg), Impact (metrics banner), Media (gallery) | Classroom learning environment |
| `quaid-e-azam.jpg` | 170 KB | Home (quote avatar), Messages (Quaid section avatar) | Quaid-e-Azam Muhammad Ali Jinnah portrait |
| `paigham-about.jpg` | 107 KB | Home (about preview), About (chairman visual), Contact (hero bg) | Paigham-e-Pakistan initiative imagery |
| `paigham-poster.jpg` | 76 KB | Messages (hero bg), Resources (hero bg), Media (gallery) | Initiative poster and branding |
| `paigham-conference.jpg` | 27 KB | Home (news), Events (launching visual, hero bg), Media (gallery, press) | Conference and launch event |
| `paigham-endorsement.jpg` | 44 KB | About (hero bg), Media (hero bg, gallery, press) | Official endorsement ceremony |
| `sindh-prisoners-education.jpg` | 45 KB | Home (news), Media (gallery, press) | Education for prisoners' children in Sindh |
| `asim-munir.jpg` | 55 KB | Messages (Field Marshal avatar) | Field Marshal Syed Asim Munir portrait |
| `prison-rehabilitation.jpg` | 57 KB | Impact (success stories banner), Media (gallery) | Prison rehabilitation programme |
| `pakistan-education.jpg` | 479 KB | Initiative (peacebuilding visual), Media (gallery) | Education in Pakistan |

### Image Placement Map

- **Home (index.html)**: Hero visual image, about preview image with overlay, 3 news card images, Quaid-e-Azam quote avatar
- **About (about.html)**: Page hero background image, chairman's section image with overlay
- **Messages (messages.html)**: Page hero background image, Quaid-e-Azam portrait avatar, Field Marshal Asim Munir portrait avatar
- **Our Initiative (initiative.html)**: Page hero background image, scholarship feature image, peacebuilding feature image
- **Events (events.html)**: Page hero background image, launching ceremony feature image
- **Impact (impact.html)**: Page hero background image, metrics section banner, success stories section banner
- **Media Center (media.html)**: Page hero background image, 4 press release card images, 8-image photo gallery with hover captions
- **Resources (resources.html)**: Page hero background image
- **Contact (contact.html)**: Page hero background image

---

## 🎨 Design & Technical Features

### Color Palette
- **Pakistan Green (Primary)**: `#01411C`
- **Gold (Accent)**: `#c5a34d`
- **Dark Primary**: `#012d14`
- **Neutrals**: Full gray scale from `#f8f9fa` to `#212529`

### Typography
- **Headings**: Playfair Display (serif)
- **Body**: Inter (sans-serif)

### Image CSS Components
- `.hero-visual-img` — Hero section image with badge overlay
- `.feature-visual-img` — Feature block image with gradient overlay caption
- `.update-card-img-real` — News/update card with image and zoom hover effect
- `.quote-author-avatar-img` — Circular author portrait with border
- `.gallery-item img` — Gallery image with hover zoom and caption fade-in
- `.page-hero-img` — Page hero section with background image and color overlay
- `.section-banner` — Full-width section banner image

### Responsive Design
- **Breakpoints**: 480px, 767px, 991px, 1199px, 1400px+
- Mobile-first responsive navigation with slide-out panel
- All images responsively sized with `object-fit: cover`
- Lazy loading on all below-fold images

### Accessibility
- Semantic HTML5 structure
- ARIA labels on interactive elements
- Descriptive `alt` text on all images
- Focus states and keyboard navigation
- Reduced motion support (`prefers-reduced-motion`)
- High contrast mode support (`prefers-contrast: high`)

### Interactive Features
- Multi-level dropdown navigation with mobile slide-out
- Scroll-triggered counter animations
- FAQ accordion
- Tab system (Resources page)
- Contact form with client-side validation
- Contact form data storage via REST API (`contact_submissions` table)
- Back-to-top button
- Sticky header with scroll shadow
- Intersection Observer animations
- Lazy image loading

---

## 📁 File Structure

```
paigham-e-pakistan/
├── index.html                  # Home page
├── about.html                  # About Us
├── messages.html               # Messages of Hope
├── initiative.html             # Our Initiative
├── events.html                 # Events & Activities
├── impact.html                 # Impact & Outcomes
├── media.html                  # Media Center
├── resources.html              # Resources
├── contact.html                # Contact & Collaboration
├── css/
│   ├── style.css               # Main styles + image components
│   └── responsive.css          # Responsive breakpoints
├── js/
│   └── main.js                 # JavaScript functionality
├── images/
│   ├── children-education.jpg
│   ├── children-classroom.jpg
│   ├── quaid-e-azam.jpg
│   ├── paigham-about.jpg
│   ├── paigham-poster.jpg
│   ├── paigham-conference.jpg
│   ├── paigham-endorsement.jpg
│   ├── sindh-prisoners-education.jpg
│   ├── asim-munir.jpg
│   ├── prison-rehabilitation.jpg
│   └── pakistan-education.jpg
├── Paigham-e-Pakistan-Magazine.pdf
└── README.md
```

---

## 📊 Data Model

### Table: `contact_submissions`
| Field | Type | Description |
|-------|------|-------------|
| id | text | Unique identifier (auto) |
| name | text | Submitter's full name |
| email | text | Submitter's email address |
| subject | text | Inquiry topic |
| message | text | Message content |
| submitted_at | datetime | Submission timestamp |

---

## 🔗 Navigation Architecture

### Main Navigation (9 items)
1. **Home** → `index.html`
2. **About Us** → `about.html` (dropdown: Chairman's Message, Vision & Mission, Our Team, FAQ, Partners)
3. **Messages** → `messages.html` (dropdown: Quaid-e-Azam, Field Marshal Asim Munir, Government Officials)
4. **Our Initiative** → `initiative.html` (dropdown: Scholarship Program, Rehabilitation, Peacebuilding, Implementation)
5. **Events** → `events.html` (dropdown: Launching Ceremony, Workshops, Scholarship Distributions)
6. **Impact** → `impact.html` (dropdown: Metrics, Success Stories, Long-term Vision)
7. **Media** → `media.html` (dropdown: Press Releases, Photo Gallery, Video Gallery)
8. **Resources** → `resources.html`
9. **Contact** → `contact.html`

### Supporting Navigation
- Top bar with email/phone and social media links
- Breadcrumb navigation on all sub-pages
- Footer with Quick Links, Programs, and Contact Info
- Back-to-top button

---

## ✅ Completed Features
- [x] All 9 main pages fully implemented with content from PDF source
- [x] Multi-level dropdown navigation with responsive mobile behavior
- [x] 11 images extracted and placed across all pages per page mapping
- [x] Image gallery in Media Center with hover effects
- [x] Page hero sections with background images
- [x] Feature visual sections with image overlays
- [x] Author portrait avatars (Quaid-e-Azam, Field Marshal)
- [x] News/update cards with real images
- [x] Complete CSS image component system
- [x] Responsive image handling across all breakpoints
- [x] Contact form with API data storage
- [x] All interactive features (counters, FAQ, tabs, animations)
- [x] Accessibility features (ARIA, alt text, keyboard nav, reduced motion)
- [x] SEO meta tags on all pages

## 🔮 Recommended Next Steps
- [ ] Source official Paigham-e-Pakistan logo from PDF or organization
- [ ] Add Urdu/English bilingual language toggle
- [ ] Integrate CMS for dynamic content management
- [ ] Add Google Analytics / site analytics
- [ ] Implement server-side form handling
- [ ] Add SSL/HTTPS for production deployment
- [ ] Create dedicated image gallery with lightbox
- [ ] Add PWA capabilities for offline access
- [ ] Implement newsletter subscription
- [ ] Add search functionality

---

## 📞 Contact Information
- **Email**: info@paighamepakistan.org
- **Phone**: 0333 2171648
- **Location**: Karachi, Sindh, Pakistan

---

## 📝 Content Source
All content is derived from the **Paigham-e-Pakistan Magazine Layout PDF** — the sole authoritative source. No facts have been invented beyond the PDF content. Content has been adapted for web readability while preserving the dignified, national-level tone and hierarchical relationships.

---

© 2026 Paigham-e-Pakistan. All rights reserved.
