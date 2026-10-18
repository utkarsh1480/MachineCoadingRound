# Assignment Round 1 — Responsive Team Dashboard

## Instructions

Please read all requirements before starting the assignment.

1. Spend the first 5–10 minutes reviewing the requirements and planning your layout.
2. Suggested implementation time: **45 minutes**.
3. Use **HTML and CSS only**. JavaScript is not required for this assessment.
4. Do not use Bootstrap, Tailwind CSS, jQuery, CSS frameworks, or other UI libraries.
5. Use a code editor such as Visual Studio Code.
6. You may consult documentation to verify HTML and CSS behavior.
7. Build the layout yourself and be prepared to explain your Flexbox decisions.
8. Test your solution at desktop, tablet, and mobile viewport sizes.

## Overview

Build a **Team Members Dashboard** named **TeamFlow**. The page contains a top navigation bar, a page heading, and a collection of team-member cards. The goal is to demonstrate practical CSS Flexbox skills, including alignment, spacing, wrapping, and responsive sizing.

## Finished App Requirements

### 1. Navigation bar

Create a horizontal navigation bar with three sections:

- **Left:** Logo and company name, `TeamFlow`.
- **Center:** `Dashboard`, `Projects`, and `Team` navigation links.
- **Right:** A profile avatar or initials and the username `Alex`.

The navigation bar should have consistent spacing and vertical alignment. Use Flexbox to arrange the sections. Do not use `100vh` to size a horizontal navigation section.

### 2. Page heading

Below the navigation bar, show:

- Heading: **Our Team**
- Subtitle: **Meet the people building great products.**
- A horizontal divider separating the navigation area from the content.

### 3. Team-member cards

Display **six team-member cards**. Each card must include:

- A circular avatar or initials.
- The member's name.
- The member's role.
- An online/offline status indicator.
- A short description.
- A `View Profile` button.

Use these sample team members:

| Name | Role | Status |
|---|---|---|
| Priya Sharma | Backend Developer | Online |
| Alex Morgan | Frontend Developer | Online |
| Sarah Chen | UI/UX Designer | Offline |
| James Wilson | Product Manager | Online |
| Rahul Verma | Full Stack Developer | Online |
| Emma Davis | QA Engineer | Offline |

Example description: `Collaborates with the team to deliver quality products.`

### 4. Responsive behavior

The cards must follow these layout requirements:

- **Desktop (above 900px):** Four cards per row.
- **Tablet (601px–900px):** Two cards per row.
- **Mobile (600px and below):** One card per row.

The page must not develop horizontal overflow at smaller viewport sizes. You may adjust the exact breakpoints if you can justify your choice.

## Flexbox requirements

Use Flexbox for the primary layout. Your solution should demonstrate:

- `display: flex`
- `justify-content`
- `align-items`
- `gap`
- `flex-wrap`
- `flex-direction`
- `flex` or `flex-basis`
- `margin-top: auto` where appropriate to align card buttons

**Do not use CSS Grid** for the navbar or the team-card collection.

## Technical constraints

- Keep markup in `index.html` and styles in `dashboard.css`.
- Prefer semantic HTML elements such as `header`, `nav`, `main`, `section`, and `article`.
- Avoid unnecessary inline styles; create reusable CSS classes instead.
- Use `box-sizing: border-box`.
- Do not set the same page background on every element using the universal selector.
- Avoid absolute positioning for the main layout.
- Ensure opening and closing HTML tags match.
- Give buttons visible hover and keyboard-focus states.
- Keep text readable and card content from overflowing.
- Use meaningful class names and consistent formatting.

## Suggested project structure

```text
teamflow-dashboard/
├── index.html
└── dashboard.css
```

## Acceptance checklist

Before finishing, confirm that:

- [ ] The navbar contains the logo, navigation links, and user profile.
- [ ] Navbar items are aligned and spaced using Flexbox.
- [ ] The heading, subtitle, and divider are present.
- [ ] All six team-member cards are displayed.
- [ ] Each card contains all required information and a button.
- [ ] Four cards fit in a desktop row.
- [ ] Two cards fit in a tablet row.
- [ ] One card fits in a mobile row.
- [ ] Cards wrap correctly and no horizontal overflow appears.
- [ ] Buttons align consistently at the bottom of the cards where space allows.
- [ ] Repeated inline styles are replaced with reusable CSS classes.
- [ ] The page uses semantic HTML and valid, matching tags.
- [ ] Buttons have hover and focus states.
- [ ] CSS Grid is not used for the main layout.

## Evaluation rubric

| Area | Points |
|---|---:|
| Flexbox usage and understanding | 25 |
| Responsive behavior | 20 |
| Navbar alignment and spacing | 15 |
| Card layout and consistency | 15 |
| HTML/CSS structure and maintainability | 15 |
| Accessibility and interaction states | 10 |
| **Total** | **100** |

## Submission

Submit the following:

1. `index.html`
2. `dashboard.css`
3. A screenshot of the desktop layout.
4. A screenshot of the mobile layout.

Name your project folder `TeamFlow-Dashboard`. Before submitting, test the page at desktop, tablet, and mobile widths.

## Interview follow-up questions

Be ready to explain:

1. What is the difference between `justify-content` and `align-items`?
2. What do the three values in `flex: 1 1 260px` mean?
3. How does `flex-wrap: wrap` affect the card collection?
4. What is the difference between `flex-basis`, `width`, and `max-width`?
5. What is the difference between `align-content` and `align-items`?
6. Why can `margin-top: auto` push a button toward the bottom of a column flex container?
7. Why is `100vh` unsuitable for sizing a horizontal navigation section?
8. How does `box-sizing: border-box` affect an element's dimensions?
9. How would you prevent long text from overflowing a card?
10. How would you make the navbar usable on mobile?

**Good luck!**
