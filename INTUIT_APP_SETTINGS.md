# Intuit QuickBooks App Settings

Complete configuration values for your Intuit Developer Portal app.

## Legal Documents (Already Completed ✓)

**End-user license agreement URL:**
```
https://babylonman.github.io/bookkeepingbyjon/eula.html
```

**Privacy policy URL:**
```
https://babylonman.github.io/bookkeepingbyjon/privacy.html
```

---

## App URLs and Domain

Since this is a **locally-run Python application** (not a web service), use these values:

### Host Domain
```
babylonman.github.io
```
*This is your GitHub Pages domain where documentation is hosted*

### Launch URL
```
https://babylonman.github.io/bookkeepingbyjon/
```
*This takes users to your app's information page*

### Disconnect URL
```
https://babylonman.github.io/bookkeepingbyjon/
```
*Same as launch URL - users return to your info page after disconnecting*

---

## App Categories

Select these categories (choose 3-4):

**Primary Categories:**
1. ✓ **Accounting** (core functionality)
2. ✓ **Data Management** (data validation and import)
3. ✓ **Income Management** (Shopify/Amazon revenue tracking)
4. ✓ **eCommerce Management** (Shopify/Amazon integration)

**Alternative Categories:**
- Expense Management (if you add fee tracking features)
- Invoicing (if you add invoice features)
- Business Insights (if you add reporting features)

---

## App Hosting Information

Since this is a **locally-installed Python application**, not a hosted web service:

### Hosting Location

**Option 1: If Required to Provide IP**
```
Country: United States
IP Type: Not applicable - Desktop application
```

**Option 2: If You Must Provide an IP**
- Enter "127.0.0.1" (localhost - indicates local installation)
- Or leave blank if the form allows it

### Explanation
This application:
- Runs on the user's local machine
- Does NOT run on a centralized server
- Connects directly from user's computer to QuickBooks API
- All data processing happens locally

---

## App Description (For Reference)

If you need to update your app description, use this:

**Short Description:**
```
QuickBooks Online data validation and reconciliation tools for e-commerce businesses using Shopify and Amazon.
```

**Long Description:**
```
Professional bookkeeping automation tools for e-commerce businesses. Validates QuickBooks Online data against Shopify and Amazon source documents, identifies missing transactions, detects duplicates, and automates payout imports.

Features:
• Complete QBO data extraction via API
• Shopify payout validation and import
• Amazon order reconciliation
• Missing transaction detection
• Duplicate identification
• Automated journal entry creation
• Comprehensive validation reports
• Local-only data processing (secure)

Perfect for:
- E-commerce businesses on Shopify/Amazon
- Bookkeepers managing multiple clients
- Businesses with incomplete QBO integrations
- Anyone needing data validation confidence

Security: All processing happens locally on your machine. We never store your financial data on servers. Uses secure OAuth 2.0 authentication with QuickBooks.
```

---

## Redirect URIs (OAuth Settings)

Make sure you have:

**Redirect URI:**
```
http://localhost:8000/callback
```

**Additional Redirect URIs (if needed):**
```
http://localhost:3000/callback
http://127.0.0.1:8000/callback
```

---

## Screenshot Requirements

If Intuit requires screenshots, you can provide:

1. **Authentication flow** - OAuth consent screen
2. **Data validation screen** - Terminal output showing validation
3. **Import results** - Success message after importing payouts
4. **Validation report** - Sample validation_report.txt

Let me know if you need help generating these screenshots.

---

## App Logo/Icon

If you need an app logo, you can:
1. Create a simple logo with your initials "BJ"
2. Use a bookkeeping-related icon (calculator, ledger book)
3. Use your business logo if you have one

Recommended size: 512x512 pixels

---

## Summary for Form Submission

Copy/paste these values into the Intuit Developer Portal:

| Field | Value |
|-------|-------|
| **EULA URL** | https://babylonman.github.io/bookkeepingbyjon/eula.html |
| **Privacy Policy URL** | https://babylonman.github.io/bookkeepingbyjon/privacy.html |
| **Host Domain** | babylonman.github.io |
| **Launch URL** | https://babylonman.github.io/bookkeepingbyjon/ |
| **Disconnect URL** | https://babylonman.github.io/bookkeepingbyjon/ |
| **Categories** | Accounting, Data Management, Income Management, eCommerce Management |
| **Hosting Country** | United States |
| **IP Address** | 127.0.0.1 (or "Not applicable - Desktop app") |

---

## Important Notes

### Desktop Application Considerations

1. **No Centralized Server**: This app runs entirely on the user's machine
2. **Local Data Only**: Financial data never leaves the user's computer
3. **Direct API Connection**: User's machine connects directly to QuickBooks API
4. **OAuth Flow**: Standard OAuth 2.0 with localhost redirect

### If Intuit Questions Hosting

If Intuit asks about hosting:
- Explain this is a **desktop/CLI application**
- Users install it on their local machines
- No centralized server involved
- Similar to QuickBooks Desktop integration pattern
- All API calls originate from user's IP address

### Production vs Development

**Development:**
- Environment: "Sandbox"
- For testing only
- Connects to test QBO companies

**Production:**
- Environment: "Production"
- Connects to real QBO companies
- Requires approved EULA and Privacy Policy ✓
- Requires app categorization ✓

---

## Next Steps After Approval

Once you get production keys:

1. Update your `.env` files with production credentials
2. Set `QBO_ENVIRONMENT=production`
3. Test with a real QuickBooks company
4. Document any production-specific setup steps

---

## Questions?

If Intuit support asks for clarification:
- Emphasize this is a **desktop application** for bookkeepers
- Similar to QuickBooks Desktop's app ecosystem
- Users install locally, not a SaaS platform
- All data processing is local for maximum security

Good luck with your production key approval!
