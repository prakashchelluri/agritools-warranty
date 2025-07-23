AgriTools Warranty Claim Portal
A simple, modern web portal for submitting agricultural equipment warranty claims.
Users can enter their details, describe their issue, and upload images. Claims are automatically logged to a Google Sheet, and images are stored securely in Cloudinary.
Features
Easy-to-use form for warranty claim submission
Image upload (multiple images supported, stored in Cloudinary)
Automatic Request ID generation for each claim
Data sent directly to Google Sheets via Google Apps Script Web App
Responsive, modern UI built with Tailwind CSS
How It Works
User fills out the form with their name, claim description, and uploads images.
Images are uploaded to Cloudinary using an unsigned upload preset.
Form data and image URLs are sent to a Google Apps Script Web App, which writes the data to a Google Sheet.
A unique Request ID is generated for each claim and shown to the user.
Setup & Deployment
1. Cloudinary Setup
Create a free Cloudinary account.
In Cloudinary dashboard, create an unsigned upload preset (e.g., unsigned_preset).
2. Google Sheets & Apps Script
Create a Google Sheet to store claims.
In the sheet, go to Extensions > Apps Script and add a script to accept POST requests and write data to the sheet.
Deploy the script as a Web App (set access to “Anyone”).
3. Configure the HTML
Set your Cloudinary cloud name and unsigned preset in the HTML.
Set your Google Apps Script Web App URL in the HTML.
4. Host the Site
You can host the index.html file for free using Netlify, GitHub Pages, or any static hosting provider.
Usage
Open the portal in your browser.
Fill in your name and claim details.
Upload one or more images (optional).
Submit the form.
You’ll receive a Request ID and your claim will be logged in the Google Sheet.
Customization
You can modify the form fields, styling, or add new features as needed.
For email notifications or more advanced workflows, consider integrating with EmailJS or similar services.
License
This project is provided as-is for personal or business use.
Feel free to modify and adapt it to your needs.
