# Deployment Guide

## Free Hosting Options

Your website is ready to deploy! Here are the easiest free options:

---

## 🚀 **Option 1: Netlify Drop (Easiest - No Account Needed)**

1. Go to https://app.netlify.com/drop
2. Drag and drop the entire `life-coaching` folder
3. Your site will be live instantly with a free URL like: `random-name-12345.netlify.app`
4. To customize the URL or connect a domain, create a free Netlify account

**Pros:** Instant, no signup needed
**Cons:** Random URL unless you create account

---

## 🚀 **Option 2: Netlify (Recommended - Best Features)**

1. Create free account at https://www.netlify.com
2. Click "Add new site" → "Deploy manually"
3. Drag the `life-coaching` folder
4. Your site is live!
5. You can customize the URL or add a custom domain for free

**Features:**
- Free SSL certificate
- Custom domain support
- Automatic deployments from Git
- Form handling (useful for contact form)
- Free subdomain: `your-site-name.netlify.app`

---

## 🚀 **Option 3: GitHub Pages**

1. Create a GitHub account at https://github.com
2. Create a new repository named `oxana-life-coaching`
3. Push your code:
   ```bash
   git remote add origin https://github.com/YOUR-USERNAME/oxana-life-coaching.git
   git branch -M main
   git push -u origin main
   ```
4. Go to repository Settings → Pages
5. Select "main" branch as source
6. Your site will be at: `your-username.github.io/oxana-life-coaching`

---

## 🚀 **Option 4: Vercel**

1. Create account at https://vercel.com
2. Click "Add New" → "Project"
3. Import from Git or drag folder
4. Your site is live at: `your-project.vercel.app`

---

## 📧 **Setting Up the Contact Form**

The contact form currently logs to console. To make it work:

### Option A: Netlify Forms (Recommended if using Netlify)
1. Add `netlify` attribute to form tag in index.html:
   ```html
   <form class="contact-form" id="contactForm" netlify>
   ```
2. Netlify will automatically handle form submissions
3. View submissions in Netlify dashboard

### Option B: Formspree
1. Sign up at https://formspree.io (free)
2. Create a form and get your endpoint
3. Update form action in index.html:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

### Option C: EmailJS
1. Sign up at https://www.emailjs.com (free)
2. Follow their setup guide
3. Update the JavaScript in `js/script.js`

---

## 🌐 **Custom Domain**

Once deployed, you can add a custom domain (like `oxanacoaching.com`):

1. Buy domain from Namecheap, Google Domains, etc. (~$10-15/year)
2. In your hosting platform (Netlify/Vercel), add custom domain
3. Update DNS settings as instructed
4. Free SSL certificate is automatically applied

---

## ✅ **Quick Deploy Now (Recommended)**

**Fastest method:**
1. Go to https://app.netlify.com/drop
2. Drag the entire folder onto the page
3. Done! Your site is live.

**To update later:**
- Drag the folder again to the same site
- Or connect to GitHub for automatic deployments

---

## 📝 **Before Going Live Checklist**

- [ ] Add real contact email in `index.html`
- [ ] Add real phone number
- [ ] Upload Oxana's professional photo to `images/oxana-profile.jpg`
- [ ] Test contact form
- [ ] Review all content for accuracy
- [ ] Check site on mobile devices
- [ ] Set up Google Analytics (optional)
- [ ] Create social media profiles and add links

---

## 🆘 **Need Help?**

All these platforms have excellent documentation and free support for deployment issues.
