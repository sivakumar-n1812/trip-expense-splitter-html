# 🧾 Trip Expense Splitter

A standalone web-based expense tracking and splitting application, similar to Splitwise. Perfect for managing shared expenses during trips with friends!

## 📋 Features

### Core Functionality
- ✅ **Friend Management** - Add/remove friends in your group
- ✅ **Expense Tracking** - Record who paid and who should split each expense
- ✅ **Smart Calculations** - Automatic balance calculations for all participants
- ✅ **Settlement Optimization** - Minimizes number of transactions needed to settle debts
- ✅ **Total Spending Overview** - See how much each person has spent
- ✅ **Spending Breakdown** - View who spent money on behalf of whom
- ✅ **CSV Export/Import** - Save and load your trip data
- ✅ **Template System** - Download pre-formatted CSV template for easy data entry

### Currency
- All amounts displayed in **Indian Rupees (₹)**

## 🚀 Getting Started

### Installation
1. Download the `trip-splitter.html` file
2. Double-click to open in any modern web browser
3. No installation or internet connection required (after first load)

### First Time Setup
The app comes pre-loaded with default friends: **Siva, Niruban, Sadheesh, Gowtham**
- You can modify, add, or remove friends as needed

## 📖 How to Use

### Adding Friends
1. Type a friend's name in the input field under "Friends" section
2. Click "Add" button or press Enter
3. To remove a friend, click the trash icon next to their name

### Adding Expenses
1. Enter a description (e.g., "Dinner", "Hotel", "Taxi")
2. Enter the amount in rupees
3. Select who paid from the dropdown
4. Click on friend names to select who should split this expense
5. Click "Add Expense" button

### Understanding the Dashboard

**Expenses Section**
- Shows all recorded expenses with details
- Displays total trip expenses
- Delete individual expenses using the trash icon

**Total Money Spent**
- Shows how much each person has paid out of pocket
- Blue cards indicate individual spending

**Spent on Others Breakdown**
- Purple cards show detailed breakdown
- Example: "Siva spent on: Niruban ₹300, Gowtham ₹450"
- Helps understand who covered expenses for whom

**Balances**
- 🟢 Green (positive) = Money owed to you
- 🔴 Red (negative) = Money you owe
- ⚫ Gray (zero) = All settled

**Settlements**
- Shows minimum transactions needed to settle all debts
- Example: "Niruban → Siva ₹500"
- Displays "All settled up! 🎉" when balanced

## 💾 Data Management

### Exporting Data
1. Click "Export to CSV" button (appears after adding expenses)
2. File downloads automatically with date stamp
3. Contains all friends, expenses, balances, and settlements

### Importing Data
1. Click "Import CSV" button
2. Select your CSV file
3. Data will be added to current session
4. Success/error message appears confirming import

### Using the Template
**Option 1: Download Template**
1. Click "Download Template" button
2. Open the CSV file in Excel/Google Sheets/Notepad
3. Edit the data following the format
4. Save and import back

**Option 2: View Template Format**
1. Click "Show Template Format" button
2. View the format directly in the app
3. Create your own CSV following this structure

### CSV Format Structure
```csv
FRIENDS
Siva,Niruban,Sadheesh,Gowtham

EXPENSES
Description,Amount,Paid By,Split Between
Dinner,1500,Siva,"Siva, Niruban, Sadheesh, Gowtham"
Movie Tickets,600,Niruban,"Niruban, Sadheesh"
Taxi,300,Gowtham,"Siva, Gowtham"
```

**Format Rules:**
- Keep section headers: `FRIENDS` and `EXPENSES`
- Friends: comma-separated names on one line
- Expenses: one per line with exact format
- "Split Between" must be in quotes with comma-separated names
- Amount should be numeric only (no ₹ symbol needed in CSV)

## ⚠️ Important Notes

### Data Persistence
- ⚠️ **Data is NOT automatically saved**
- All data is lost when you close the browser tab
- **Always export your data before closing!**
- Import your CSV file to restore data in a new session

### Browser Compatibility
- Works on all modern browsers (Chrome, Firefox, Safari, Edge)
- Requires JavaScript enabled
- Responsive design - works on mobile and desktop

### Best Practices
1. **Regular Exports** - Export data frequently during long trips
2. **Backup Files** - Keep multiple dated CSV backups
3. **Verify Imports** - Check expense count after importing
4. **Clear Descriptions** - Use clear expense descriptions for easy reference
5. **Real-time Updates** - Add expenses as they happen to avoid forgetting

## 🔧 Technical Details

### Technology Stack
- **Frontend**: React 18 (via CDN)
- **Styling**: Tailwind CSS (via CDN)
- **Format**: Standalone HTML file
- **Storage**: Browser memory (session-based)

### File Size
- Single HTML file (~15-20 KB)
- Loads external libraries from CDN on first run
- Works offline after initial load

### Dependencies
- React 18 (CDN: cdnjs.cloudflare.com)
- React DOM 18 (CDN: cdnjs.cloudflare.com)
- Babel Standalone (CDN: cdnjs.cloudflare.com)
- Tailwind CSS (CDN: cdn.tailwindcss.com)

## 🐛 Troubleshooting

### Import Issues
**Problem**: Expenses not importing
**Solution**: Make sure your CSV follows the exact format with proper quotes around "Split Between" field

**Problem**: "No valid data found"
**Solution**: Check that FRIENDS and EXPENSES section headers are present

### Display Issues
**Problem**: App shows raw code instead of interface
**Solution**: Make sure file is saved as .html extension and opened in a browser

### Calculation Issues
**Problem**: Balances seem incorrect
**Solution**: Verify that "Split Between" includes all correct people for each expense

## 💡 Tips & Tricks

1. **Quick Split All**: When adding an expense, click all friends for equal split
2. **Partial Splits**: Select only specific people who participated in an activity
3. **Track Categories**: Use descriptive names like "Food-Dinner" or "Transport-Taxi"
4. **Regular Reviews**: Check settlements section regularly to settle debts
5. **Document Everything**: Take photos of receipts and note them in descriptions


## 📄 License

Free to use and modify for personal use.

---

## 🎉 Happy Trip Planning!

Enjoy your trips without the hassle of calculating who owes whom. Split expenses fairly and transparently with your friends!

---

**Version**: 1.0  
**Last Updated**: December 2024  
**Default Friends**: Siva, Niruban, Sadheesh, Gowtham
