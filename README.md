# Online Science Festival Schedule

A responsive web page that shows the program schedule of an online science festival, organized by date tabs.
Built with plain HTML, CSS, and vanilla JavaScript.

## Features

- **Date tabs**: The schedule covers 13 weekdays, from November 24 to December 10. Click a date tab to see that day's programs.
- **Program cards**: Each card shows the time, program title, host organization, and an image. Card colors (blue, pink, orange) mark the target audience: All Ages, Grades 1+, and Grades 6+.
- **Favorites**: Click the heart button to mark a program you're interested in, and click again to unmark it.
- **Responsive layout**: The layout changes at 1200px, 1000px, and 767px, so the page works on desktop, tablet, and mobile. On smaller screens, a weekday header (Mon–Fri) appears above the date tabs.

## Tech Stack

- HTML5
- CSS3 (responsive design with media queries)
- JavaScript (ES6, no libraries)

## Project Structure

```
scienceday-schedule/
├── schedule.html            # Main page (markup + tab/heart scripts)
├── css/
│   └── style.schedule.css   # Page styles
└── scienceImages/           # Program images
    ├── science01.png
    ├── science02.png
    └── science03.png
```

## Getting Started

No build step is needed. Download the repository and open `schedule.html` in your browser.

## How It Works

- Each tab in `.planTab` links to the schedule section for its date with `href="#planN"`, which points to the element `#planN`.
- When the page loads, every schedule section is hidden except the one for the tab with the `planOpen` class (November 24).
- Clicking a tab moves the `active` class to that tab and shows only the matching schedule section.
- Clicking a `.heart_btn` turns its `active` class on or off.

## Author

- sumin
