# Rate Management System

A simple 4-page web application for managing product rate submissions with customer and admin portals.

## Features

### Customer Portal
- **Login Page**: Email and password authentication
- **Rate Submission Form**: Submit product rates with automatic market analysis
- **Real-time Analysis**: Instant feedback on rate competitiveness

### Admin Portal
- **Admin Login**: Separate authentication for administrators
- **Review Dashboard**: View all customer submissions
- **Approval System**: Approve or reject rate submissions
- **Filtering**: Filter by status (pending, approved, rejected)

## File Structure

```
├── index.html              # Main landing page
├── customer-login.html     # Customer login page
├── admin-login.html        # Admin login page
├── customer-form.html      # Rate submission form
├── admin-review.html       # Admin review dashboard
├── styles.css              # Common styling
├── users.json             # User credentials (static)
└── submissions.json       # Customer submissions data
```

## Demo Credentials

### Customer Accounts
- **Email**: customer1@example.com | **Password**: password123
- **Email**: customer2@example.com | **Password**: password456

### Admin Accounts
- **Email**: admin1@example.com | **Password**: admin123
- **Email**: admin2@example.com | **Password**: admin456

## How to Run

1. Open `index.html` in a web browser
2. Choose either Customer or Admin login
3. Use the demo credentials provided above
4. Navigate through the application

## Features Breakdown

### Rate Analysis System
The system includes intelligent rate analysis that:
- Compares submitted rates against market rates by country
- Provides automatic recommendations (approve/reject)
- Categorizes rates as Competitive, Premium, High, or Below Market
- Calculates percentage difference from market standards

### Data Storage
- User credentials stored in `users.json`
- Submissions stored in `submissions.json` initially
- New submissions saved to browser localStorage for demo purposes
- Real-time updates between customer submissions and admin reviews

### Security Features
- Session management using localStorage
- Route protection (redirects if not logged in)
- Separate authentication for customers and admins

### User Experience
- Responsive design works on desktop and mobile
- Real-time form validation
- Success/error messaging
- Auto-refresh functionality
- Clean, modern interface

## Browser Compatibility

Works with all modern browsers that support:
- ES6 JavaScript features
- CSS Grid and Flexbox
- localStorage API
- Fetch API

## Technical Implementation

- **Frontend**: Pure HTML, CSS, JavaScript (no frameworks)
- **Data**: JSON files for demo data
- **Storage**: localStorage for runtime data persistence
- **Styling**: CSS Grid, Flexbox, and CSS custom properties
- **Authentication**: Simple email/password matching against JSON data

## Future Enhancements

Potential improvements for production use:
- Backend API integration
- Database storage
- JWT authentication
- File upload functionality
- Email notifications
- Advanced reporting features
- User management system