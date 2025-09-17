# CoreyShop Email Automation

This Netlify Function sends weekly marketing emails to all subscribers using SendGrid.

## Setup Instructions

1. Sign up for a free SendGrid account: https://sendgrid.com
2. Create an API key in SendGrid.
3. On Netlify, go to Site Settings → Environment Variables and add:
   - SENDGRID_API_KEY=your_api_key_here
   - FROM_EMAIL=noreply@coreyshop.com (or your verified sender email)
4. Upload your subscribers into `subscribers.csv`.
5. Deploy this folder to Netlify connected to your GitHub repo.
6. Enable Netlify Scheduled Functions to run `send_weekly_email.js` weekly.

Edit `emails.json` to update or add new templates.
