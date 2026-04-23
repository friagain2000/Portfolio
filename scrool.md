# Role: Expert Full-stack Developer (UI/UX Specialist)
# Context: Developing a high-end portfolio for "Designer & Developer Shin Seong-min"
# Goal: Implement a 'Sticky Stacking Card' scroll effect with 4 project cards.

## 1. Requirement: Scroll Animation Logic (GSAP & ScrollTrigger)
- Create a stacking effect where 4 cards (.portfolio-item) overlap as the user scrolls.
- As a new card slides over the previous one, the previous card should:
  1) Scale down to 0.92.
  2) Decrease opacity to 0.4.
  3) Apply a subtle blur (3px) for a depth-of-field effect.
- Each card must contain an image with a 'Parallax' effect (moving 15% on the Y-axis inside its container).

## 2. Requirement: Visual & Layout (Toss-style Minimalism)
- Design the cards using a 2-column grid (Info on left, Image on right).
- Use 'Pretendard' font with letter-spacing: -0.02em.
- Color Palette: 
  - Background: #F8F9FA
  - Card: #FFFFFF (Border-radius: 32px)
  - Primary Text: #191F28
  - Accent: #3182F6 (Toss Blue)
- Button Style: Minimal chips with a light gray background (#F2F4F6) and line icons.

## 3. Tech Stack & Optimization
- Use GSAP 3.x and ScrollTrigger.
- Optimization: Use 'will-change: transform' for smooth 60fps performance.
- CSS: Use 'position: sticky' for the card containers.

## 4. Output
- Provide clean, modular HTML, CSS, and GSAP JavaScript code.
- Add comments explaining how to adjust the 'scrub' and 'start/end' values for fine-tuning.