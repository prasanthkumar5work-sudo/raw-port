# EmailJS Setup Guide

## ✅ Step 1: Create EmailJS Account (FREE)

1. Go to https://www.emailjs.com/
2. Click **"Sign Up"** (top right)
3. Sign up with your Google account (prasasnthkumar5work@gmail.com)
4. Verify your email

## ✅ Step 2: Add Email Service

1. After login, click **"Add New Service"**
2. Select **"Gmail"**
3. Click **"Connect Account"**
4. Sign in with: **prasasnthkumar5work@gmail.com**
5. Allow EmailJS permissions
6. **Copy the Service ID** (looks like: `service_abc1234`)

## ✅ Step 3: Create Email Template

1. Go to **"Email Templates"** tab
2. Click **"Create New Template"**
3. Use this template:

```
Subject: New Portfolio Contact from {{from_name}}

From: {{from_name}}
Email: {{from_email}}

Message:
{{message}}
```

4. Click **"Save"**
5. **Copy the Template ID** (looks like: `template_xyz5678`)

## ✅ Step 4: Get Public Key

1. Go to **"Account"** → **"General"**
2. Find **"Public Key"** section
3. **Copy your Public Key** (looks like: `aBcD1234eFgH5678`)

## ✅ Step 5: Update Your Code

Open: `src/components/Contact.jsx`

Find these lines (around line 15-17):

```javascript
const serviceID = 'YOUR_SERVICE_ID';
const templateID = 'YOUR_TEMPLATE_ID';
const publicKey = 'YOUR_PUBLIC_KEY';
```

Replace with YOUR actual values:

```javascript
const serviceID = 'service_abc1234';  // Your Service ID
const templateID = 'template_xyz5678'; // Your Template ID
const publicKey = 'aBcD1234eFgH5678';  // Your Public Key
```

## ✅ Step 6: Test It!

1. Save the file
2. Refresh your browser
3. Fill out the contact form
4. Click "Send Message"
5. Check your Gmail inbox!

## 🎉 Done!

Now visitors can send you emails directly without opening their email client!

**FREE Plan Limits:**
- 200 emails/month
- Perfect for a portfolio website!

## ❓ Need Help?

If you get stuck, the EmailJS dashboard has great documentation and support!
