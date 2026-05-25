# NIELIT Study Centre Phayeng - Web Portal

## 📌 Overview
A comprehensive web application for NIELIT Study Centre Phayeng with student registration, admin management, course management, payment tracking, and notifications system.

## ✨ Features

### Public Features
- 🏠 Home page with statistics and latest notifications
- 📚 Course catalog with search
- 📝 Online registration with photo upload
- 🔍 Application status tracking
- 💳 Fee payment system
- 🎥 Photo & video gallery
- 👨‍🎓 Student login portal

### Student Dashboard
- View personal details
- Check application status
- View payment status
- See payment history
- Track course enrollment

### Admin Features
- 👨‍💼 Complete admin dashboard
- 📊 Statistics and analytics
- ✏️ **Full Edit Capabilities:**
  - Edit all student details (name, email, mobile, DOB, gender, qualification, course, batch, fee, status, payment status, registration date, address)
  - Edit payment records (amount, date, method, transaction ID)
  - Edit notifications (title, content, priority, category)
  - Edit courses (name, duration, fee, description)
- ➕ Add new students, courses, notifications, payments
- 🗑️ Delete any records
- 🔍 Search and filter functionality

## 🚀 Deployment Options

### Option 1: GitHub Pages (FREE & RECOMMENDED)

#### Step-by-Step Guide:

1. **Create a GitHub Account** (if you don't have one)
   - Go to https://github.com
   - Click "Sign up"

2. **Create a New Repository**
   - Click the "+" icon in the top right
   - Select "New repository"
   - Name it: `nielit-portal` (or any name you prefer)
   - Make it **Public**
   - Click "Create repository"

3. **Upload Your File**
   - Click "uploading an existing file"
   - Drag and drop `nielit-portal.html`
   - Rename it to `index.html` (important!)
   - Click "Commit changes"

4. **Enable GitHub Pages**
   - Go to repository Settings
   - Scroll to "Pages" in left sidebar
   - Under "Source", select "main" branch
   - Click "Save"
   - Wait 1-2 minutes

5. **Access Your Website**
   - Your site will be live at: `https://YOUR-USERNAME.github.io/nielit-portal/`

---

### Option 2: Netlify (FREE)

1. **Sign up at Netlify**
   - Go to https://www.netlify.com
   - Sign up (free account)

2. **Deploy**
   - Drag and drop the `nielit-portal.html` file (rename to `index.html`)
   - Or connect your GitHub repository
   - Your site will be live instantly!
   - You'll get a URL like: `https://random-name-12345.netlify.app`

3. **Custom Domain (Optional)**
   - You can use a custom domain for free
   - Settings → Domain management

---

### Option 3: Vercel (FREE)

1. **Sign up at Vercel**
   - Go to https://vercel.com
   - Sign up with GitHub

2. **Deploy**
   - Click "New Project"
   - Import your GitHub repository
   - Deploy!
   - Live at: `https://your-project.vercel.app`

---

### Option 4: Firebase Hosting (FREE)

1. **Create Firebase Project**
   - Go to https://firebase.google.com
   - Create new project

2. **Install Firebase CLI**
   ```bash
   npm install -g firebase-tools
   firebase login
   firebase init hosting
   ```

3. **Deploy**
   ```bash
   firebase deploy
   ```

---

### Option 5: Render (FREE)

1. Go to https://render.com
2. Sign up (free account)
3. Click "New Static Site"
4. Connect GitHub or upload file
5. Deploy!

---

## 🔑 Default Login Credentials

### Admin Login
- **Username:** `admin`
- **Password:** `admin123`

### Student Login
- Use Registration ID + Email from any registered student

---

## 📝 How to Use

### For Students:
1. Go to **Registration** tab
2. Fill out the form with your details
3. Upload your photo
4. Submit
5. Note your Registration ID
6. Use **Student Login** to access your dashboard

### For Admin:
1. Login with admin credentials
2. **View & Edit Students:**
   - Click "Edit" button on any student
   - Modify any field including fees, dates, status
   - Save changes
3. **Manage Courses:**
   - Click "Manage Courses"
   - Add, edit, or delete courses
4. **Manage Notifications:**
   - Click "+ Add Notification"
   - Edit or delete existing notifications
5. **Manage Payments:**
   - Edit payment amounts and details
   - Delete payment records

---

## 🔧 Customization

### Change Admin Password
Open `index.html` and find this line (around line 1450):
```javascript
if (username === 'admin' && password === 'admin123') {
```
Change `'admin123'` to your desired password.

### Change Header Colors
Find the `.header` style section and modify the gradient:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #f093fb 100%);
```

### Add Your Logo
Replace the header text with an image:
```html
<img src="your-logo.png" alt="NIELIT Logo" style="max-width: 300px;">
```

---

## 💾 Data Storage

- All data is stored in browser's **localStorage**
- Data persists even after closing browser
- Each browser/device has separate data
- To backup data: Use browser's developer tools to export localStorage

### Export Data (for backup):
1. Press F12 to open Developer Tools
2. Go to "Console" tab
3. Type:
```javascript
console.log(JSON.stringify(localStorage));
```
4. Copy the output

### Import Data (restore backup):
1. Paste your backup data
2. Parse and set each item back to localStorage

---

## 🌐 Custom Domain (Optional)

All free hosting platforms above support custom domains:

1. Buy a domain from:
   - Namecheap ($8-15/year)
   - Google Domains ($12/year)
   - Freenom (FREE .tk, .ml, .ga domains)

2. Point domain to your hosting:
   - GitHub Pages: Add CNAME file
   - Netlify/Vercel: Add domain in settings
   - Follow platform-specific guides

---

## 📱 Mobile Responsive

The portal is fully responsive and works perfectly on:
- Desktop computers
- Tablets
- Mobile phones

---

## 🔒 Security Notes

**For Production Use:**
1. Change default admin password
2. Implement proper backend authentication
3. Use a database instead of localStorage
4. Add HTTPS (automatic on all platforms above)
5. Implement password hashing
6. Add email verification

---

## 🆘 Support

For issues or questions:
1. Check browser console for errors (F12)
2. Ensure JavaScript is enabled
3. Try clearing browser cache
4. Use modern browsers (Chrome, Firefox, Edge, Safari)

---

## 📄 License

Free to use and modify for educational purposes.

---

## 🎉 Quick Start

**Fastest Way to Deploy (2 minutes):**

1. Rename `nielit-portal.html` to `index.html`
2. Go to https://app.netlify.com/drop
3. Drag and drop the `index.html` file
4. Done! Your site is live!

---

## ✅ What Admin Can Edit

### Student Records
✅ Full Name
✅ Email
✅ Mobile Number
✅ Date of Birth
✅ Gender
✅ Qualification
✅ Course
✅ Batch Timing
✅ Application Status
✅ Payment Status
✅ Fee Amount
✅ Registration Date
✅ Address
✅ Delete Student

### Payments
✅ Registration ID
✅ Student Name
✅ Payment Amount
✅ Payment Method
✅ Transaction ID
✅ Payment Date
✅ Delete Payment

### Notifications
✅ Title
✅ Content
✅ Priority Level
✅ Category
✅ Link
✅ Delete Notification

### Courses
✅ Course Name
✅ Duration
✅ Fee Amount
✅ Description
✅ Delete Course

**Everything is editable by admin!**

---

## 🔄 Updates & Maintenance

To update your deployed site:
1. Make changes to `index.html`
2. Upload to your hosting platform
3. Changes appear immediately (or after cache clear)

---

**Developed for NIELIT Study Centre Phayeng**
*An Autonomous Society under Ministry of Electronic & Information Technology, Govt. of India*
