# 📊 Elegant Landscape Habit Tracker

A beautifully designed web-based habit tracking application that helps you build and monitor your daily habits. Track multiple habits throughout the month with an interactive A4 landscape view, customize themes, and export your progress as a printable PDF or JSON backup.

## ✨ Features at a Glance

- **📅 Monthly Habit Tracking**: Create a customizable monthly tracker for any number of habits
- **🎨 6 Beautiful Themes**: Choose from professionally designed themes to match your style
- **📑 Print-Ready PDFs**: Download your habit tracker in landscape A4 format, ready to print
- **💾 Export & Import**: Save your habit configurations and progress as JSON backups
- **✅ Interactive Tracking**: Click cells to mark habits as completed for each day
- **🔍 Live Preview**: See real-time changes as you customize your tracker
- **📱 Responsive**: Works seamlessly on desktop browsers
- **⚙️ Zoom Control**: Adjust the preview size to fit your screen perfectly

## 🚀 Getting Started

### Opening the Application

1. Navigate to the `atomic-habits` folder
2. Open the `index.html` file in your web browser
3. The application will load with a clean, welcoming interface

The app uses **localStorage** to persist your changes, so your habits and progress are saved automatically.

---

## 📖 How to Use the Application

### Step 1️⃣: Initial Setup

When you first open the application, you'll see the **Setup Page**:

#### **What to Configure:**

1. **Tracker Title**
   - Enter a name for your habit tracker (e.g., "Monthly Habits", "April Goals", "Fitness Challenge")
   - This title appears at the top of your printed tracker
   - Default: "Monthly Habits"

2. **Month Selection**
   - Choose which month you want to track (January through December)
   - The calendar automatically adjusts to show the correct number of days
   - Select based on when you want to start tracking

3. **Year**
   - Enter the year for your tracker
   - This ensures your exported data is properly dated
   - Default: Current year (2026)

**Example Setup:**
```
Title: "Fitness & Wellness April"
Month: April
Year: 2026
```

Once you've configured these settings, click the **"Continue →"** button to proceed to Step 2.

---

### Step 2️⃣: Adding Habits & Customization

After clicking Continue, you'll enter the **Habits Management Page** where you can:

#### **Add Habits**

1. Look for the **"Add New Habit"** field at the top
2. Type your habit name (e.g., "Exercise", "Drink Water", "Read", "Meditate")
3. Press **Enter** or click the **"+"** button to add the habit
4. Your habit will appear in both the habit list and the tracker table
5. Repeat for all habits you want to track

**Habit Examples:**
- Exercise (30 mins)
- Drink 8 glasses of water
- Read 20 pages
- Meditate
- Take vitamins
- Journal writing
- Morning stretches
- Sleep before 11 PM

#### **Remove Habits**

- Each habit in the list has a red **"Delete"** button next to it
- Click to remove a habit from your tracker
- Removing a habit also removes all checked cells for that habit

---

### Step 3️⃣: Mark Your Progress

In the main **A4 Tracker Preview**, you can interactively track your habits:

1. **Understand the Table Structure:**
   - **Left column**: Habit names
   - **Top row**: Days of the month (1-28, 1-30, or 1-31)
   - **Cells**: Click to toggle between completed ✓ and uncompleted

2. **Marking Progress:**
   - Click on any cell to mark the habit as completed for that day
   - The cell will change color (appears "checked") based on your selected theme
   - Click again to unmark if you made a mistake
   - Changes are saved automatically

3. **Real-Time Updates:**
   - As you add or remove habits, the table updates instantly
   - The number of days adjusts based on the selected month

---

### Step 4️⃣: Choose Your Theme

Customize the look and feel of your tracker with one of **6 professional themes**:

#### **Theme Gallery:**

| Theme Name | Description | Best For |
|-----------|-----------|----------|
| **Sleek Professional** | Classic black and white, clean and minimal | Office environments, formal tracking |
| **Warm Sunset (Pastel)** | Soft peachy and warm tones | Cozy, comfortable tracking experience |
| **Modern Mint (Rounded)** | Fresh mint green with rounded corners | Modern, friendly aesthetic |
| **Ocean Wave (Curved)** | Calming blue tones with curved, floating cells | Relaxing, stress-free tracking |
| **Soft Berry (Super Rounded)** | Romantic pink/berry with ultra-rounded design | Creative, personal projects |
| **Forest Bubble (Floating/Curved)** | Natural yellow-green with bubble-like cells | Nature-inspired, organic feel |

**Theme Features:**
- Each theme adjusts colors, spacing, and borders
- Checked cells change color to match the theme
- Headers and accents are specifically designed for each theme
- Themes are purely visual - no impact on functionality

**To Switch Themes:**
1. Locate the **"Theme"** dropdown menu
2. Click to see all available themes
3. Select your preferred theme
4. The preview updates instantly

---

## 🖨️ Exporting Your Tracker

### Download as PDF

Perfect for printing or sharing your habit tracker:

1. Click the **"Download Landscape PDF"** button
2. Your browser will download the file as `habit-tracker.pdf`
3. The PDF will be in **A4 landscape format** (297mm × 210mm)
4. All theme colors and formatting are preserved
5. Open with any PDF reader or send to a printer

**Tips:**
- Print at 100% scale for proper sizing
- Use quality paper (white or colored) for best results
- Print double-sided to save paper (odd pages on one side, even on back)
- Laminate for a reusable tracker (use dry-erase markers)

---

### Export Data as JSON

Save your habits and progress for backup or transfer:

1. Click the **"Export Data (.json)"** button
2. A file named `Habit-Backup-[timestamp].json` will download
3. This file contains:
   - Your tracker title, month, and year
   - All habit names
   - All checked cells (completed days)
   - App version information

**Exported JSON Structure:**
```json
{
  "app": "HabitTracker",
  "version": "1.1",
  "title": "Monthly Habits",
  "month": 4,
  "year": 2026,
  "habits": ["Exercise", "Read", "Meditate"],
  "checkedCells": ["0-1", "0-2", "1-1", "2-5"]
}
```

---

## 📥 Importing Saved Data

Restore previous trackers or transfer data:

### Import Options

1. **Full Import** (All Data):
   - Restores habits, progress, title, month, and year
   - Uncheck the "Only Habits" option
   - Click **"Import File"** and select your JSON backup

2. **Habits-Only Import**:
   - Restores only habit names
   - Keeps your current month/year and progress
   - Check the **"Only Habits"** checkbox first
   - Useful for reusing the same habit set for different months

### Import Steps

1. Click **"Import File"** button in the initial setup screen
2. Select your previously exported `.json` file
3. The app validates the file format
4. Habits are loaded, and you're ready to continue

**Important Notes:**
- Only `.json` files generated by this app can be imported
- Importing automatically takes you to Step 2
- You can still modify habits after importing
- Imported data doesn't overwrite your current month/year unless you select full import

---

## 🔍 Preview Controls

### Zoom Feature

Adjust the preview size to fit your screen:

1. **Zoom Slider** (top-right of preview):
   - Drag to zoom from 30% to 100%
   - Or click and type a percentage
   - Zooming is for preview only - doesn't affect PDF quality

2. **Zoom Display**:
   - Shows current zoom percentage (e.g., "50%", "75%")
   - Updates in real-time

**When to Adjust Zoom:**
- Zoom in (80-100%) to see details better
- Zoom out (30-50%) to see the entire tracker at once
- Find your preferred zoom level for comfortable tracking

---

## 📝 Complete Workflow Diagram

```
┌─────────────────────────────────────────────────────────────────┐
│                    START: Open index.html                        │
└────────────────┬────────────────────────────────────────────────┘
                 │
                 ▼
         ┌───────────────┐
         │   STEP 1:     │
         │  Enter Setup  │
         └───────┬───────┘
                 │
         ┌───────▼─────────┐
         │ Set Tracker:    │
         │ • Title         │
         │ • Month         │
         │ • Year          │
         └───────┬─────────┘
                 │
         ┌───────▼──────────────┐
         │ Click "Continue →"   │
         └───────┬──────────────┘
                 │
                 ▼
         ┌───────────────────┐
         │    STEP 2:        │
         │ Manage Habits     │
         └───────┬───────────┘
                 │
     ┌───────────┼───────────┐
     │           │           │
     ▼           ▼           ▼
┌─────────┐ ┌────────┐ ┌──────────┐
│ Add     │ │Choose  │ │ Preview  │
│ Habits  │ │ Theme  │ │ Updates  │
└────┬────┘ └────┬───┘ └──────┬───┘
     │           │            │
     └───────────┼────────────┘
                 │
                 ▼
         ┌───────────────┐
         │ Track Daily   │
         │ Progress      │
         │ (Click Cells) │
         └───────┬───────┘
                 │
         ┌───────▼──────────────┐
         │  Export/Download:    │
         │  • Download PDF      │
         │  • Export JSON       │
         └──────────────────────┘
```

---

## 💡 Tips & Best Practices

### Creating Effective Habits

- **Be Specific**: Instead of "Exercise", use "30-minute run" or "Strength training"
- **Keep it Simple**: 3-7 habits per tracker is ideal for focus
- **Start Small**: Build momentum with achievable habits before adding more
- **Mix Categories**: Combine physical, mental, and emotional habits

### Using the Tracker Effectively

- **Print Weekly**: Print a single week to carry with you
- **Color It In**: Print and use colored markers to make it engaging
- **Track Immediately**: Mark habits the same day you complete them
- **Review Weekly**: Each Sunday, review your progress and reflect

### Organizing Your Data

- **Monthly Backups**: Export data after completing each month
- **Naming Convention**: Use dates in filenames: `Habits-Apr2026-Backup.json`
- **Folder System**: Create a folder like `My-Habits/2026/` to organize files
- **Version Control**: Keep the original export and updates separate

---

## ❓ Frequently Asked Questions

### General Questions

**Q: Is my data stored online?**
- A: No! All data is stored locally in your browser using localStorage. Your information never leaves your computer.

**Q: Can I access my tracker on a different device?**
- A: Yes, export your data as JSON and import it on another device using the Import feature.

**Q: How many habits can I track at once?**
- A: There's no hard limit, but 5-10 habits per month is recommended for readability and focus.

**Q: Does this app require internet?**
- A: No, the app works entirely offline. It only needs internet to load the page initially.

### Tracking Questions

**Q: What if I forget to mark a day?**
- A: Simply click the cell for that day later. You can update anytime before exporting.

**Q: Can I track multiple months at once?**
- A: Create separate trackers for different months and export each one as an individual PDF.

**Q: What happens if I delete a habit?**
- A: The habit is removed from the table, and all progress for that habit is deleted. This cannot be undone.

### Export & Print Questions

**Q: Can I edit the PDF after downloading?**
- A: The PDF is read-only. To modify, go back to the app, make changes, and re-download.

**Q: What printer settings should I use?**
- A: Use "Landscape" orientation, "Fit to Page" or 100% scale, and normal quality for home printing.

**Q: Can I laminate and reuse the printed tracker?**
- A: Yes! Print on slightly thicker paper, laminate it, and use dry-erase markers to reuse monthly.

### Data & Backup Questions

**Q: What if my browser data gets cleared?**
- A: If you clear browser cache, your data will be lost. Always keep exported JSON files as backups.

**Q: Can I import a JSON file from a previous version?**
- A: Yes, as long as it's in the correct format (created by this app).

**Q: How do I recover a deleted habit?**
- A: If you exported before deletion, import that file to recover it. Otherwise, it's lost.

---

## 🎯 Common Use Cases

### Use Case 1: Personal Wellness
**Setup:**
- Title: "April Wellness Goals"
- Habits: Exercise, Drink Water, Sleep 8hrs, Meditate, Read
- Theme: Ocean Wave (calm & motivating)
- Export: Monthly PDF for wall display

### Use Case 2: Student Study Plan
**Setup:**
- Title: "Exam Prep - Biology"
- Habits: Study 2hrs, Review notes, Practice problems, Attend class
- Theme: Modern Mint (fresh & energetic)
- Export: Weekly PDFs for tracking progress

### Use Case 3: Team Accountability
**Setup:**
- Title: "Team Wellness Initiative"
- Habits: Team standup, Exercise, Hydration, Mental break
- Theme: Forest Bubble (natural & engaging)
- Export: Monthly trackers for team members

### Use Case 4: Habit Challenge
**Setup:**
- Title: "30-Day Writing Challenge"
- Habits: Write 1000 words, Publish post, Edit previous work
- Theme: Soft Berry (creative & personal)
- Export: Daily printouts for motivation wall

---

## 🌐 Browser Compatibility

This application works best on:
- ✅ Chrome/Chromium (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ⚠️ Mobile browsers (layout may be cramped)

For the best experience, use a **desktop or laptop** with a screen width of at least **1200px**.

---

## 📱 Responsive Design Notes

- **Desktop (1600px+)**: Full preview at optimal scale
- **Laptop (1200-1600px)**: Compact layout with adjusted preview
- **Mobile (< 1200px)**: Not optimized; use desktop for best experience

---

## 🛠️ Troubleshooting

### Issue: Habits not saving
**Solution:** Enable cookies and local storage in your browser settings. Clear cache and reload.

### Issue: PDF downloads but looks wrong
**Solution:** Ensure you're using 100% print scale and landscape orientation in your printer settings.

### Issue: Import not working
**Solution:** Verify the JSON file:
- Was created by this app
- Has `.json` extension
- Is not corrupted or incomplete

### Issue: Theme colors not visible
**Solution:** Disable dark mode in your browser or clear cached CSS. Try a different theme.

### Issue: Zoom slider not responding
**Solution:** Click directly on the range input, or use arrow keys after clicking it.

---

## 📄 File Formats

### JSON Backup Format
- **Extension**: `.json`
- **Generated by**: "Export Data" button
- **Contains**: Habits, progress, metadata
- **Used for**: Backup, transfer, recovery

### PDF Export Format
- **Format**: A4 Landscape
- **Dimensions**: 297mm × 210mm
- **Quality**: High-resolution (JPEG 0.98 quality)
- **Used for**: Printing, sharing, archival

---

## ✅ Quick Start Checklist

- [ ] Open `index.html` in your browser
- [ ] Enter tracker title (e.g., "April Habits")
- [ ] Select month and year
- [ ] Click "Continue →"
- [ ] Add your first habit
- [ ] Add more habits (3-7 recommended)
- [ ] Choose your favorite theme
- [ ] Click on cells to mark progress
- [ ] Download PDF or export JSON backup
- [ ] Print and display your tracker!

---

## 🎨 Customization Tips

### Optimizing for Your Workflow

1. **For Printing**:
   - Choose high-contrast themes (Midnight, Ocean, Berry)
   - Zoom to 100% for accurate print preview
   - Export a month's tracker as PDF immediately after setup

2. **For Digital Tracking**:
   - Use lighter themes (Pastel, Mint) for comfortable screen viewing
   - Keep 5-7 habits max for daily tracking
   - Review progress weekly

3. **For Team Use**:
   - Use professional themes (Midnight, Ocean)
   - Keep habit names short and clear
   - Export as JSON for sharing with team members

---

## 📞 Support & Feedback

If you encounter issues or have suggestions:
1. Check the **FAQ** section above
2. Review the **Troubleshooting** guide
3. Verify your browser is up-to-date
4. Ensure JavaScript is enabled

---

## 🏆 Version Information

- **Current Version**: 1.1
- **Last Updated**: 2026
- **App Name**: Elegant Landscape Habit Tracker

---

**Happy habit tracking! 🎯✨**