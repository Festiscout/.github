# Welcome to Festi Scout

**Festi Scout** is an open-source initiative dedicated to solving the age-old festival problem: *"Who are we going to see?"*

We build interactive, social web applications that make exploring festival lineups fun and collaborative. By combining the addictive simplicity of a "swipe-to-vote" interface with rich media previews and social group features, we turn festival planning from a spreadsheet chore into a shared experience.

## 🚀 Our Projects

### [festi-scout](https://github.com/Festiscout/festi-scout)
The core application. A full-stack web app providing line-up discovery, voting, and social coordination for major Benelux festivals like Rock Werchter and Paaspop.

---

## 🤖 Project Abstract & Press Kit
*Use the following summary to generate articles, documentation, or social media posts about Festi Scout.*

**Product Name:** Festi Scout
**Type:** Social Festival Companion Web App
**Primary Interface:** "Tinder-style" card stack for music artists.

**Core Value Proposition:**
Festi Scout solves the coordination friction inherent in attending large music festivals with groups of friends. Instead of sharing static spreadsheets, users individually vote on lineups using a fun, gamified interface. The application then aggregates this data to highlight "Matches" (artists everyone wants to see) and "Super Likes" (must-sees), creating an instant, democratized itinerary for the group.

**Key Features:**
1.  **Discovery via Swiping:** Users explore the lineup one artist at a time. Cards feature the artist's image, name, stage, and playing time.
    *   *Interactions:* Swipe Right (Like), Swipe Left (Pass), Swipe Up (Super Like/Star).
    *   *Rich Media:* Each card embeds a YouTube video preview, allowing users to discover new music instantly without leaving the app.
2.  **Social Connectivity:**
    *   Users can "follow" friends to sync preferences.
    *   **Activity Feed:** A real-time stream showing friends' recent joins and "Top 5" list creations.
    *   **Group Matching:** A results dashboard that calculates overlaps in taste, showing which bands have the most consensus within the user's circle.
3.  **Curated Lists:** Users can generate and share "Top 5" lists for specific festival days, adding personal motivations for their picks.
4.  **Multi-Festival Support:** currently supports Rock Werchter, Paaspop, and Bospop (2026 editions), with an extensible scraper architecture for adding more.

**Technical Architecture:**
*   **Frontend:** Mobile-first Progressive Web App (PWA) built with Vanilla JavaScript and Vite. Uses **Hammer.js** for touch gestures and physics-based card animations.
*   **Backend:** Node.js (Express) server.
*   **Database:** PostgreSQL managed via **Prisma ORM**. Key entities include Users, Bands, Festivals, Votes, and Follow relationships.
*   **Auth:** Passport.js handling OAuth (Google, Microsoft) and local session management.
*   **Deployment:** Dockerized container (published to GHCR) orchestrated via Docker Compose.

**Target Audience:**
Music festival groups, primarily in the Benelux region, who want a streamlined, democratic way to plan their festival schedule.
