🧾 Trip Expense Splitter
A standalone web-based expense tracking and splitting application, similar to Splitwise. Perfect for managing shared expenses during trips with friends!
📋 Features
Core Functionality

✅ Friend Management - Add/remove friends in your group
✅ Expense Tracking - Record who paid and who should split each expense
✅ Smart Calculations - Automatic balance calculations for all participants
✅ Settlement Optimization - Minimizes number of transactions needed to settle debts
✅ Total Spending Overview - See how much each person has spent
✅ Spending Breakdown - View who spent money on behalf of whom
✅ CSV Export/Import - Save and load your trip data
✅ Template System - Download pre-formatted CSV template for easy data entry

Currency

All amounts displayed in Indian Rupees (₹)

🚀 Getting Started
Installation

Download the trip-splitter.html file
Double-click to open in any modern web browser
No installation or internet connection required (after first load)

First Time Setup
The app comes pre-loaded with default friends: Siva, Niruban, Sadheesh, Gowtham

You can modify, add, or remove friends as needed

📖 How to Use
Adding Friends

Type a friend's name in the input field under "Friends" section
Click "Add" button or press Enter
To remove a friend, click the trash icon next to their name

Adding Expenses

Enter a description (e.g., "Dinner", "Hotel", "Taxi")
Enter the amount in rupees
Select who paid from the dropdown
Click on friend names to select who should split this expense
Click "Add Expense" button

Understanding the Dashboard
Expenses Section

Shows all recorded expenses with details
Displays total trip expenses
Delete individual expenses using the trash icon

Total Money Spent

Shows how much each person has paid out of pocket
Blue cards indicate individual spending

Spent on Others Breakdown

Purple cards show detailed breakdown
Example: "Siva spent on: Niruban ₹300, Gowtham ₹450"
Helps understand who covered expenses for whom

Balances

🟢 Green (positive) = Money owed to you
🔴 Red (negative) = Money you owe
⚫ Gray (zero) = All settled

Settlements

Shows minimum transactions needed to settle all debts
Example: "Niruban → Siva ₹500"
Displays "All settled up! 🎉" when balanced

💾 Data Management
Exporting Data

Click "Export to CSV" button (appears after adding expenses)
File downloads automatically with date stamp
Contains all friends, expenses, balances, and settlements

Importing Data

Click "Import CSV" button
Select your CSV file
Data will be added to current session
Success/error message appears confirming import

Using the Template
Option 1: Download Template

Click "Download Template" button
Open the CSV file in Excel/Google Sheets/Notepad
Edit the data following the format
Save and import back

Option 2: View Template Format

Click "Show Template Format" button
View the format directly in the app
Create your own CSV following this structure

CSV Format Structure
csvFRIENDS
Siva,Niruban,Sadheesh,Gowtham

EXPENSES
Description,Amount,Paid By,Split Between
Dinner,1500,Siva,"Siva, Niruban, Sadheesh, Gowtham"
Movie Tickets,600,Niruban,"Niruban, Sadheesh"
Taxi,300,Gowtham,"Siva, Gowtham"
Format Rules:

Keep section headers: FRIENDS and EXPENSES
Friends: comma-separated names on one line
Expenses: one per line with exact format
"Split Between" must be in quotes with comma-separated names
Amount should be numeric only (no ₹ symbol needed in CSV)

⚠️ Important Notes
Data Persistence

⚠️ Data is NOT automatically saved
All data is lost when you close the browser tab
Always export your data before closing!
Import your CSV file to restore data in a new session

Browser Compatibility

Works on all modern browsers (Chrome, Firefox, Safari, Edge)
Requires JavaScript enabled
Responsive design - works on mobile and desktop

Best Practices

Regular Exports - Export data frequently during long trips
Backup Files - Keep multiple dated CSV backups
Verify Imports - Check expense count after importing
Clear Descriptions - Use clear expense descriptions for easy reference
Real-time Updates - Add expenses as they happen to avoid forgetting

🔧 Technical Details
Technology Stack

Frontend: React 18 (via CDN)
Styling: Tailwind CSS (via CDN)
Format: Standalone HTML file
Storage: Browser memory (session-based)

File Size

Single HTML file (~15-20 KB)
Loads external libraries from CDN on first run
Works offline after initial load

Dependencies

React 18 (CDN: cdnjs.cloudflare.com)
React DOM 18 (CDN: cdnjs.cloudflare.com)
Babel Standalone (CDN: cdnjs.cloudflare.com)
Tailwind CSS (CDN: cdn.tailwindcss.com)

🐛 Troubleshooting
Import Issues
Problem: Expenses not importing
Solution: Make sure your CSV follows the exact format with proper quotes around "Split Between" field
Problem: "No valid data found"
Solution: Check that FRIENDS and EXPENSES section headers are present
Display Issues
Problem: App shows raw code instead of interface
Solution: Make sure file is saved as .html extension and opened in a browser
Calculation Issues
Problem: Balances seem incorrect
Solution: Verify that "Split Between" includes all correct people for each expense
💡 Tips & Tricks

Quick Split All: When adding an expense, click all friends for equal split
Partial Splits: Select only specific people who participated in an activity
Track Categories: Use descriptive names like "Food-Dinner" or "Transport-Taxi"
Regular Reviews: Check settlements section regularly to settle debts
Document Everything: Take photos of receipts and note them in descriptions

📄 License
Free to use and modify for personal use.

🎉 Happy Trip Planning!
Enjoy your trips without the hassle of calculating who owes whom. Split expenses fairly and transparently with your friends!

Version: 1.0
Last Updated: December 2024
