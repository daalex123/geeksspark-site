# EmailJS Setup Guide

## Step 1: Create EmailJS Account
1. Go to [https://www.emailjs.com/](https://www.emailjs.com/)
2. Sign up for a free account
3. Verify your email address

## Step 2: Create Email Service
1. In your EmailJS dashboard, go to "Email Services"
2. Click "Add New Service"
3. Choose your email provider (Gmail, Outlook, etc.)
4. Follow the setup instructions for your provider
5. Note down your **Service ID**

## Step 3: Create Email Template
1. Go to "Email Templates" in your dashboard
2. Click "Create New Template"
3. Use this template content:

**Subject:** New Contact Form Submission from {{from_name}}

**Content:**
```
Hello,

You have received a new contact form submission:

Name: {{from_name}}
Email: {{from_email}}
Company: {{company}}
Service Interested In: {{service}}

Message:
{{message}}

Best regards,
GeeksSpark Website
```

4. Save the template and note down your **Template ID**

## Step 4: Get Public Key
1. Go to "Account" in your EmailJS dashboard
2. Find your **Public Key** in the API Keys section

## Step 5: Update the Code
Replace these placeholders in your `index.html` file:

- Replace `YOUR_PUBLIC_KEY` with your actual public key
- Replace `YOUR_SERVICE_ID` with your service ID
- Replace `YOUR_TEMPLATE_ID` with your template ID

## Step 6: Test the Form
1. Open your website
2. Fill out the contact form
3. Submit it
4. Check if you receive the email at dhemantha2@gmail.com

## Troubleshooting
- Make sure all IDs are correct
- Check browser console for any errors
- Verify your email service is properly configured
- Ensure the template variables match the code

## Free Tier Limits
- 200 emails per month
- Perfect for small to medium websites
- Upgrade for higher limits if needed
