# CodeXCrakes - Lost & Found Campus Hub

This repository contains the **baby3** project - a Lost & Found Campus Hub application.

## 🚀 Deployment

### Netlify Deployment

This project is configured for automatic deployment on Netlify.

#### Quick Deploy

1. **Fork or Clone** this repository
2. **Connect to Netlify:**
   - Go to [Netlify](https://netlify.com)
   - Click "Add new site" → "Import an existing project"
   - Connect your GitHub account
   - Select this repository
   - Netlify will auto-detect the configuration from `netlify.toml`
3. **Deploy!** 
   - Click "Deploy site"
   - Your site will be live at `https://[your-site-name].netlify.app`

#### Manual Configuration

If needed, use these settings:
- **Build command:** (leave empty)
- **Publish directory:** `baby3`
- **Base directory:** (leave empty)

## 📁 Project Structure

```
baby3/
├── index.html              # Main Lost & Found portal
├── login.html              # Authentication page
├── admin-dashboard.html    # Admin management interface
└── recycle-bin.html        # Deleted items management
```

## 🔑 Default Login Credentials

- **Username:** `admin`
- **Password:** `admin123`

⚠️ **Security Note:** Change these credentials for production use!

## 🛠️ Technology Stack

- **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
- **Styling:** Tailwind CSS (CDN)
- **Storage:** localStorage (client-side)
- **Charts:** Chart.js (for admin dashboard)

## 🌟 Features

- ✅ Report lost items
- ✅ Report found items
- ✅ Search and filter items
- ✅ Admin dashboard with analytics
- ✅ Recycle bin for deleted items
- ✅ Dark/Light theme toggle
- ✅ Responsive design

## 📝 Usage

1. Access the login page
2. Enter credentials (default: admin/admin123)
3. Post lost or found items
4. Search through listings
5. Mark items as found/resolved
6. View admin analytics (admin dashboard)

## 🤝 Contributing

Made with ❤️ by **CodeXCrakes**

---

**Note:** This is a client-side application using localStorage. All data is stored locally in the browser.
