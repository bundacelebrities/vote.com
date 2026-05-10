# Bunda Celebrities Voting Platform

A modern, professional, and secure voting platform for the Bunda Celebrities Awards 2025/2026, built with international standards in mind.

## Features

- **Real-time Voting**: Live updates using Firebase Firestore
- **Live Leaderboard**: Dynamic top performers display
- **Mobile-First Design**: Fully responsive across all devices
- **Accessibility Compliant**: WCAG 2.1 AA standards
- **Rate Limiting**: Prevents vote manipulation
- **Phone Validation**: Tanzanian number verification
- **Engagement Animations**: Confetti and notifications
- **Secure Payments**: Integrated with local mobile money providers
- **International Standards**: Clean code, semantic HTML, modern CSS

## Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Backend**: Firebase Firestore (NoSQL database)
- **Styling**: Custom CSS with responsive design
- **Animations**: Canvas Confetti, CSS transitions
- **Deployment**: Static hosting (Vercel, Netlify, etc.)

## Setup Instructions

### 1. Firebase Configuration
- Create a Firebase project at [Firebase Console](https://console.firebase.google.com/)
- Enable Firestore Database and Authentication
- Update the Firebase config in `js/app.js` with your project credentials
- **Security Note**: Use environment variables for production deployment

### 2. Database Structure
Create a Firestore collection called `contestants` with documents like:
```json
{
  "name": "Contestant Name",
  "category": "Msanii Bora wa Kiume (Mara Region)",
  "image": "https://example.com/photo.jpg",
  "votes": 0
}
```

### 3. Payment Integration
- Currently simulates payment processing
- Integrate with actual gateways: M-Pesa, Airtel Money, Mixx By Yas, Halopesa
- Update payment logic in `js/app.js`

### 4. Deployment
- Host on secure web servers with HTTPS
- Add CSP headers for security
- Implement server-side validation

## Security Considerations

- Firebase config exposed in client (demo only)
- No user authentication (add OAuth for production)
- Basic rate limiting (upgrade to server-side)
- Input validation on both client and server
- HTTPS mandatory for payment processing

## Development

### File Structure
```
bundacelebrities-voting/
├── index.html          # Homepage
├── voting.html         # Voting page
├── css/
│   └── style.css       # Stylesheet
├── js/
│   └── app.js          # Application logic
├── images/             # Static assets
└── README.md           # Documentation
```

### Contributing
- Follow semantic HTML practices
- Use BEM methodology for CSS
- Write clean, commented JavaScript
- Test on multiple devices and browsers

## License

© 2025/2026 Bunda Celebrities Awards. All rights reserved.

## Technologies Used

- HTML5, CSS3, JavaScript (ES6+)
- Firebase Firestore
- Canvas Confetti for animations
- Google Fonts

## Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is for educational purposes. Modify and use as needed.