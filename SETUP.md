# Oninova Linktree App - Setup Guide

Your linktree app is ready! Follow these steps to customize it with your personal information.

## 🚀 Quick Start

The development server is already running at: **http://localhost:3000**

## 📝 Customization Steps

### 1. Update Your Profile Information

Open `app/page.tsx` and update the `profile` object (lines 5-17) with your details:

```typescript
const profile = {
  name: "Your Full Name",              // Update with your name
  title: "Sales Representative",        // Already set
  company: "Oninova",                   // Already set
  phone: "+1 (555) 000-0000",          // Update with your phone number
  image: "/profile.jpg",                // Keep this, but replace the image (see step 2)
  links: {
    linkedin: "https://linkedin.com/in/yourprofile",     // Your LinkedIn profile URL
    instagram: "https://instagram.com/yourprofile",       // Your Instagram handle
    website: "https://oninova.com",                       // Oninova website or your personal site
    whatsapp: "https://wa.me/15550000000",               // See WhatsApp format below
  },
};
```

### 2. Add Your Profile Picture

Replace the placeholder profile image:

1. Get a professional profile photo (square format works best)
2. Save it as `profile.jpg` in the `public/` folder
3. The image will automatically be displayed with a circular frame

**Recommended specs:**
- Format: JPG or PNG
- Size: 400x400px or larger (square)
- File size: Under 500KB

### 3. WhatsApp Link Format

The WhatsApp link should use this format:
```
https://wa.me/[country_code][phone_number]
```

**Example:**
- US number: +1 555-123-4567 → `https://wa.me/15551234567`
- UK number: +44 7123 456789 → `https://wa.me/447123456789`

**Remove:**
- Spaces
- Dashes
- Parentheses
- Plus sign

### 4. Social Media Links

Update each social link with your actual profiles:

- **LinkedIn:** Right-click your LinkedIn profile → Copy link to profile
- **Instagram:** Your Instagram URL is `https://instagram.com/[your_username]`
- **Website:** Use your company website or personal portfolio

## 🎨 Design Features

Your linktree includes:

✅ **Profile Section**
- Circular profile photo with black border
- Name, title, and company display
- Clickable phone number

✅ **Social Links**
- WhatsApp button with yellow (#FFFB00) accent
- LinkedIn, Instagram, and Website buttons
- Bold shadows and hover effects for a modern, corporate look

✅ **Color Scheme**
- Primary: Black & White
- Accent: Yellow (#FFFB00)
- Minimalistic and professional design

## 🛠️ Development Commands

```bash
# Run development server
npm run dev

# Build for production
npm run build

# Start production server
npm start
```

## 🌐 Deployment

When you're ready to deploy:

1. **Vercel (Recommended)**
   ```bash
   npm install -g vercel
   vercel
   ```

2. **Netlify**
   - Connect your Git repository
   - Build command: `npm run build`
   - Publish directory: `.next`

3. **Other Platforms**
   - Most platforms that support Next.js will work
   - Use `npm run build` to create a production build

## 📱 Mobile Responsive

The design is fully responsive and looks great on:
- Desktop computers
- Tablets
- Mobile phones

## 🎯 Next Steps

1. ✏️ Update your profile information in `app/page.tsx`
2. 🖼️ Replace `public/profile.jpg` with your photo
3. 🔗 Test all your links work correctly
4. 🚀 Deploy to your preferred hosting platform

## 💡 Tips

- Use a professional headshot for your profile picture
- Test your WhatsApp link before deploying
- Make sure all social links are public and accessible
- Consider shortening long URLs if needed

---

**Need help?** Check the main [README.md](README.md) or Next.js documentation at [nextjs.org](https://nextjs.org/)
