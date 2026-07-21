# How Local R U? Quiz

A interactive quiz to calculate your L.O.C.A.L. score (0-10) based on your connection to your local community.

**Live Site:** [quiz.hyperlocaldispatch.com](https://quiz.hyperlocaldispatch.com)

## About

The Local Formula was developed by [K. L. Graywill](https://www.hyperlocaldispatch.com/about) for the Hyperlocal Dispatch July 2026 edition "The Hyperlocal Habit: A Practical Guide to Finding Belonging Anywhere."

The quiz measures six key variables:
- **L1 - Lifespan**: How long you've lived in your area
- **θ - Outreach**: How active you are in local activities
- **H - Hyperlocal Factor**: Your average daily travel distance
- **C - Compass**: Your navigation knowledge of the area
- **A - Authenticity**: Your connection to local culture and issues
- **L2 - Lore**: Your knowledge of local history

## Project Structure

```
Hyperlocal/
├── index.html              # Main quiz page
├── assets/
│   ├── fonts/             # Custom typewriter fonts
│   ├── hyperlocal masthead.png
│   └── hyperlocal generic map gradient.png
├── how-local-r-u.html     # Original widget version
└── README.md
```

## Features

- Mobile-optimized interface with large tap targets
- Custom handwritten and typewriter fonts
- Interactive multi-step quiz with progress tracking
- Local flair assignment based on your responses
- Score sharing functionality
- **Coming Soon**: Zipcode-based community statistics
- **Coming Soon**: Compare your score with your area

## Deployment

This site is deployed via **GitHub Pages** and accessible at a custom subdomain.

### GitHub Pages Setup
1. Push to GitHub repository
2. Go to Settings > Pages
3. Source: Deploy from `main` branch, `/` (root) folder
4. Custom domain: `quiz.hyperlocaldispatch.com`

### DNS Configuration (Namecheap)

To set up the subdomain `quiz.hyperlocaldispatch.com`:

1. Log in to Namecheap
2. Go to Domain List > Manage for `hyperlocaldispatch.com`
3. Advanced DNS tab
4. Add new CNAME Record:
   - **Host**: `quiz`
   - **Value**: `klgraywill.github.io` (or your GitHub Pages URL)
   - **TTL**: Automatic

5. In GitHub repo settings, add custom domain `quiz.hyperlocaldispatch.com`
6. Wait for DNS propagation (up to 24 hours, usually faster)

## Future Backend Integration

The quiz is designed to easily integrate with either:
- **Firebase** (Firestore + Cloud Functions)
- **Supabase** (PostgreSQL + REST API)

Backend features will include:
- Zipcode-based score aggregation
- Local flair distribution statistics
- Data export for analysis
- User consent and privacy controls

## Development

To work on this locally:
1. Clone the repository
2. Open `index.html` in a browser
3. No build process required - pure HTML/CSS/JS

## Credits

- **Quiz Design & Formula**: K. L. Graywill
- **Math Support**: Alex Kritchevsky and Andrew Evans
- **Publisher**: [Hyperlocal Dispatch](https://hyperlocaldispatch.com)
- **Support on Patreon**: [patreon.com/c/klgraywill](https://www.patreon.com/c/klgraywill)

## License

© 2026 K. L. Graywill / Hyperlocal Dispatch. All rights reserved.
