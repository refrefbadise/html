# Heineken Reporting Dashboard

A complete password-protected reporting dashboard for tracking Heineken campaign activities including customer engagements, sales, giveaways, check-ins/check-outs, and photo uploads.

## Features

✅ **Password Protected Login** - Secure access with session authentication
✅ **Campaign Dashboard** - Real-time view of all submissions
✅ **Data Submission Form** - Easy form to submit campaign reports
✅ **Photo Management** - Upload and view check-in/check-out photos
✅ **Admin Panel** - Backend data management and export
✅ **Data Analytics** - Stats cards, summaries, and filters
✅ **Multiple Export Formats** - JSON and CSV data export
✅ **Responsive Design** - Works on desktop, tablet, and mobile
✅ **Local Data Storage** - No server required, all data stored locally in browser

## Tracked Metrics

- **Customer Engagements** - Count of customers engaged
- **Sales Made** - Number of sales transactions
- **Giveaways Distributed** - Number of promotional items given
- **Check-in/Check-out Times** - Time tracking for each session
- **Photos** - Visual evidence (check-in and check-out photos)
- **Location** - Campaign location
- **Promoter Name** - Name of the person running the campaign
- **Outlets Checked In** - List of outlets/stores visited

## File Structure

```
heineken-dashboard/
├── index.html          # Login page
├── dashboard.html      # Main dashboard (view all reports)
├── form.html           # Submit new report
├── admin.html          # Admin panel (backend data view)
├── styles.css          # All styling
└── README.md           # This file
```

## How to Use

### 1. Access the Dashboard

- Open `index.html` in your web browser
- **Default Password**: `Heineken2026`
- You can change the password by editing line 33 in `index.html`

### 2. Submit a Report

1. Click "+ New Report" on the dashboard
2. Fill in all required fields:
   - Report Date
   - Promoter Name
   - Location
   - Outlets Checked In
   - Engagement metrics (customer engagements, sales, giveaways)
   - Check-in time (auto-filled)
   - Check-out time (optional)
   - Upload photos
3. Click "Submit Report"

### 3. View Reports

- The dashboard automatically displays all submitted reports
- Search by location, promoter, or outlet
- View detailed information by clicking "View" on any report
- See check-in and check-out photos in the gallery

### 4. Manage Backend Data

- Click "Admin Panel" link to view backend data
- View all data in JSON format
- Export data as JSON or CSV
- View summary statistics by promoter
- Clear data if needed

## Sharing via WhatsApp

Once deployed, you can share the dashboard link via WhatsApp:

### Local Testing
- Open the folder in a local server (Python, Node.js, etc.)
- Share the localhost URL

### Production Deployment (GitHub Pages)
1. Enable GitHub Pages in your repository settings
2. Select the branch with the `heineken-dashboard` folder
3. GitHub will provide a public URL to share
4. Share the link via WhatsApp

### Example Sharing Message
```
🍺 Heineken Campaign Dashboard
Access your reporting portal here: [YOUR_URL]/heineken-dashboard/

Password: Heineken2026

Track engagements, sales, giveaways, and more!
```

## Data Storage

All data is stored locally in your browser's **localStorage**:
- No data is sent to any server
- Data persists even after closing the browser
- Data is device-specific (not synced across devices)
- Can be manually backed up via admin panel export

## Security Notes

⚠️ **Important**: This dashboard uses:
- **Session authentication** (password verification on login)
- **Client-side storage** (no server required)
- **Client-side encryption** (none - use HTTPS in production)

For production use:
- Change the default password
- Deploy over HTTPS
- Consider adding server-side authentication
- Implement proper data encryption

## Browser Compatibility

- ✅ Chrome/Chromium (Recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## Customization

### Change Password
Edit line 33 in `index.html`:
```javascript
const DASHBOARD_PASSWORD = "Heineken2026"; // Change this
```

### Customize Logo
Replace the Heineken logo URLs with your own image URLs

### Adjust Colors
Edit CSS variables in `styles.css`:
```css
--primary-color: #00a651;
--primary-dark: #008040;
--secondary-color: #f7b600;
```

## Troubleshooting

**Q: Data disappeared after closing browser**
- A: Check if you're using incognito/private browsing mode (data won't persist)
- Use regular browsing mode instead

**Q: Photos not showing**
- A: Photos are stored as base64 in localStorage (size limited)
- For large photo collections, export regularly and archive

**Q: Password not working**
- A: Check that you typed the password exactly (case-sensitive)
- Clear browser cache and try again

**Q: Can't access admin panel**
- A: Make sure you're logged in first
- Go back to dashboard, then click "Admin Panel" link

## Support

For issues or suggestions, contact your administrator.

---

**Created for**: Heineken Campaign Management
**Version**: 1.0
**Last Updated**: 2026-05-08