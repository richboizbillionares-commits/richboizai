# NexusAI - Interactive Prototype

A professional, interactive prototype for NexusAI - an AI tools platform for small businesses. This prototype demonstrates the user interface and user flow for investors, customers, and developers.

## 🚀 Quick Start

### Opening the Prototype

1. **Download the file**: Ensure you have `index.html` saved locally
2. **Open in browser**: Double-click `index.html` or right-click and select "Open with" → Your preferred browser
3. **Best experience**: Use Chrome, Firefox, Safari, or Edge (latest versions)

That's it! No server, no installation, no dependencies needed.

## 📱 Browser Requirements

- **Recommended**: Chrome 90+, Firefox 88+, Safari 14+, Edge 90+
- **Internet connection**: Required for Tailwind CSS and Lucide Icons (loaded via CDN)
- **Screen size**: Best viewed on desktop (1024px+), but fully responsive for tablet and mobile

## 🎯 How to Demo

### Screen 1: Pricing Tiers
**What it shows**: Three pricing tiers for different business sizes

**Actions to try**:
- Hover over each pricing card (watch the subtle scale animation)
- Click "Select Starter" or "Select Professional" → Navigate to tool selection
- Click "Contact Sales" → Opens contact modal
- Click "Or build your own package →" → Navigate to tool selection
- Notice the "Most Popular" badge with glow effect on Professional plan

### Screen 2: Tool Selection Dashboard
**What it shows**: Six AI tools available for à la carte selection

**Actions to try**:
- Click anywhere on a tool row (except checkbox) → Expands to show detailed features
- Click the checkbox → Selects/deselects the tool
- Watch the **real-time price calculation** in header and bottom bar
- Select 3+ tools → See "Save with Professional plan" message
- Try selecting/deselecting multiple tools → Notice smooth animations
- Click "Continue to Setup →" (enabled when ≥1 tool selected)

**Tools available**:
1. AI Receptionist - $99/mo
2. AI Website Builder - $79/mo
3. AI Booking System - $69/mo
4. AI Email Assistant - $89/mo
5. AI Customer Chat - $79/mo
6. AI Social Media - $89/mo

### Screen 3: Business Configuration
**What it shows**: Form to collect business information

**Actions to try**:
- Fill out the form fields
- **Required fields**: Business Name, Industry, Phone, Primary Location
- **Optional field**: Website (notice the helper text)
- Watch the "Review & Deploy" button - stays disabled until all required fields are filled
- Try leaving a required field empty → Button remains disabled
- Click "← Back to Tools" → Returns to tool selection (data is preserved)
- Notice the progress indicator at top showing Step 2 as active

**Form validation**:
- Real-time validation as you type
- Button enables only when all required fields are valid

### Screen 4: Review & Confirm
**What it shows**: Final review before "deployment"

**Sections to review**:
1. **Selected AI Tools**: Lists all chosen tools with prices
   - Click "Edit" next to any tool → Return to tool selection
2. **Business Information**: Displays entered data in clean grid
   - Click "Edit" button → Return to configuration screen
3. **Payment Information**: Mock payment form (prototype only)
   - Shows 14-day free trial message
   - Displays trial end date (automatically calculated)

**Actions to try**:
- Review the total price calculation
- Notice the progress indicator (Steps 1 & 2 completed, Step 3 active)
- Try the Edit buttons to go back and modify selections
- Click "← Back to Configure" → Return to previous screen
- Click "Deploy All Tools 🚀" → Shows loading state, then navigates to success screen

### Screen 5: Success / Confirmation
**What it shows**: Celebration of successful deployment

**Actions to try**:
- Notice the pulsing checkmark animation
- See the list of deployed tools with "✓ Active" status
- Click "View Dashboard" → Navigate to the Management Dashboard (Screen 6)
- Click "Download Setup Guide" → Coming soon alert
- Click "← Start Over" → Confirms, then resets everything and returns to pricing

### Screen 6: Management Dashboard
**What it shows**: Central control panel for managing all deployed AI tools

**Sections**:
1. **Top Navigation**: Logo, menu items (Dashboard, AI Tools, Analytics, Settings, Billing), user avatar
2. **Overview Stats**:
   - Active Tools count (dynamically shows number of selected tools)
   - Tasks Automated Today: 142
   - Estimated Monthly Savings: $2,847
   - Subscription Status (shows actual subscription price)
3. **Your AI Tools Grid**: Cards for each deployed tool showing:
   - Tool name and icon
   - Active status indicator
   - Real-time stats (calls handled, visitors, appointments, etc.)
   - View Details and Configure buttons
4. **Recent Activity Feed**: Timeline of activities from your deployed tools
5. **Quick Actions**: Buttons to add tools, view analytics, update settings, contact support

**Actions to try**:
- Hover over tool cards → See scale animation
- Click navigation menu items → "Coming soon" alerts (except Dashboard which is active)
- Click user avatar → Coming soon alert
- Click "View Details" on any tool → Coming soon alert
- Click "Configure" on any tool → Coming soon alert
- Click quick action buttons → Various "coming soon" alerts
- Click "Manage billing" → Coming soon alert
- Notice that only the tools you selected are displayed in the grid
- Notice the active tool count matches your selection

**Dynamic Features**:
- Tool count and subscription price update based on your selections
- Only tools you selected during setup are shown
- Activity feed shows activities only for tools you deployed

## 🔄 Data Persistence

The prototype uses **localStorage** to save your progress:

- **Selected tools** are remembered
- **Business information** is saved
- **Current screen** is preserved

This means if you refresh the page or close/reopen the browser, your selections persist!

### How to Reset/Clear Data

**Option 1: Use "Start Over" button**
- Navigate to the Success screen (Screen 5)
- Click "← Start Over"
- Confirm the dialog
- All data cleared, returns to Screen 1

**Option 2: Clear browser localStorage**
- Open browser DevTools (F12)
- Go to "Application" tab (Chrome) or "Storage" tab (Firefox)
- Find "Local Storage" → Your domain
- Delete the `nexusai-state` item
- Refresh the page

**Option 3: Use browser console**
```javascript
localStorage.removeItem('nexusai-state');
location.reload();
```

## 🎨 Design Features

### Color Palette
- **Primary Dark**: #0f172a (slate-900) - main backgrounds
- **Secondary Dark**: #1e293b (slate-800) - cards/panels
- **Accent Blue**: #3b82f6 (blue-500) - primary actions
- **Accent Cyan**: #06b6d4 (cyan-500) - highlights/selected states
- **Text Primary**: #f1f5f9 (slate-100)
- **Text Secondary**: #94a3b8 (slate-400)

### Key Design Elements
- Modern, dark SaaS aesthetic (inspired by Stripe, Linear, Vercel)
- Smooth transitions and hover effects
- Custom checkboxes with animations
- Responsive design (mobile, tablet, desktop)
- Generous spacing and clean typography
- Subtle shadows and glows
- Professional, minimal style

## 🛠 Technical Details

### Tech Stack
- **HTML5**: Semantic markup
- **Tailwind CSS**: Via CDN for rapid styling
- **Vanilla JavaScript**: No frameworks, pure JS
- **Lucide Icons**: Via CDN for beautiful line icons
- **Inter Font**: Via Google Fonts

### File Structure
```
nexusai-prototype/
├── index.html          # Single file containing everything
└── README.md          # This file
```

### Features Implemented
✅ 6 complete screens with smooth navigation
✅ Real-time price calculations
✅ Interactive tool selection with expand/collapse
✅ Form validation with real-time feedback
✅ Progress indicators
✅ LocalStorage for data persistence
✅ Fully responsive design
✅ Smooth animations and transitions
✅ Modal dialogs
✅ Loading states
✅ Custom checkbox styling
✅ Hover effects and focus states
✅ Accessible keyboard navigation

## 📋 Screen Flow Summary

```
Screen 1: Pricing Tiers
    ↓ (Select plan OR "Build your own")
Screen 2: Tool Selection
    ↓ (Select tools → Continue)
Screen 3: Configuration
    ↓ (Fill form → Review & Deploy)
Screen 4: Review & Confirm
    ↓ (Deploy All Tools)
Screen 5: Success
    ↓ (View Dashboard)
Screen 6: Management Dashboard
    ↓ (Start Over → Returns to Screen 1)
```

## 🎯 What This Prototype Demonstrates

### For Investors
- Professional, polished user interface
- Clear value proposition with pricing tiers
- Flexible à la carte model
- Smooth user experience
- Modern, trustworthy design

### For Customers
- Simple, intuitive flow
- Transparent pricing
- Easy tool selection
- No technical knowledge required
- Clear next steps

### For Developers
- Clean, maintainable code
- Well-structured JavaScript
- Responsive design patterns
- State management with localStorage
- Reusable components

## ⚠️ Limitations (This is a Prototype)

- **No backend**: No real data processing or API calls
- **No database**: Data only stored in browser localStorage
- **No authentication**: No login or user accounts
- **No payment processing**: Payment form is for show only
- **No actual AI tools**: This demonstrates the purchasing flow only
- **Limited form validation**: Basic validation, not production-ready
- **Mock contact modal**: Sales contact is just an alert

## 🐛 Troubleshooting

### Icons not showing
- Check internet connection (icons load from CDN)
- Try refreshing the page
- Check browser console for errors

### Styles look broken
- Check internet connection (Tailwind CSS loads from CDN)
- Try a different browser
- Clear cache and refresh

### Data not persisting
- Check if localStorage is enabled in your browser
- Check if you're in private/incognito mode (localStorage is cleared on close)
- Try clearing localStorage and starting fresh

### Button not enabling
- Ensure all required fields are filled
- Check browser console for JavaScript errors

## 📝 Notes

- This prototype is designed to be **portable** - just the single HTML file
- No build process or dependencies needed
- Works offline after initial load (CDN resources cached)
- Fully self-contained for easy sharing and demoing

## 🎉 Demo Script (For Presentations)

1. **Start**: "This is NexusAI, an AI tools platform for small businesses"
2. **Screen 1**: "Businesses can choose from three preset plans, or build their own"
3. **Click "Build your own"**
4. **Screen 2**: "Here they select exactly which AI tools they need" - Click a few tools, show expand
5. **Watch price update**: "Notice the price updates in real-time as they select tools"
6. **Click Continue**
7. **Screen 3**: "We collect basic business info to customize their experience"
8. **Fill form quickly**
9. **Screen 4**: "They review everything before deployment" - Show edit buttons
10. **Click Deploy**
11. **Screen 5**: "And they're live! All tools are deployed and ready to use"
12. **Click "View Dashboard"**
13. **Screen 6**: "Here's their management dashboard - see only the tools they selected, real-time stats, activity feed, and quick actions"

Total demo time: ~3-4 minutes

## 📧 Questions?

This is a prototype only. For questions about the actual NexusAI product, contact: contact@nexusai.com

---

**Built with attention to detail** ✨
No templates. No shortcuts. Just clean, professional code.
