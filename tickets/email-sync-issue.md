cat << 'EOF' > tickets/email-sync-issue.md
# Ticket Scenario: Email Not Syncing (Outlook / Microsoft 365)

## Ticket Summary
A user reports that their email is not syncing in Outlook. New emails are not appearing.

## Ticket Details
- Ticket Type: Email / Cloud Services
- Priority: Medium
- Platform: Microsoft Outlook / Microsoft 365
- Device: Windows 10/11 Laptop
- Status: Resolved

## User Complaint
The user states that Outlook is open, but no new emails are appearing. Other users are receiving emails normally.

## Initial Assessment
Possible causes include:
- Outlook offline mode
- poor internet connectivity
- corrupted Outlook profile
- mailbox sync issue
- credential/authentication issue
- Exchange server delay

## Troubleshooting Steps

### 1. Verify internet connectivity
- Open Command Prompt and run:

ping google.com

- Confirmed successful replies

---

### 2. Check Outlook connection status
- Open Outlook
- Checked bottom status bar

Observed:
- Outlook showed "Disconnected" / "Trying to connect"

---

### 3. Disable Work Offline mode
- In Outlook, go to Send/Receive tab
- Checked if "Work Offline" is enabled
- Disabled it if active

---

### 4. Restart Outlook
- Closed Outlook completely
- Reopened the application

---

### 5. Check account settings
- File → Account Settings → Account Settings
- Verified correct email account
- Checked server settings

---

### 6. Test Outlook Web Access (OWA)
- Logged into email via browser (Outlook Web)

Result:
- Emails were updating correctly in browser

---

### 7. Recreate Outlook profile
- Open Control Panel → Mail
- Created new Outlook profile
- Re-added email account

---

## Root Cause
The Outlook application had a corrupted or desynchronized profile, preventing proper email syncing.

## Resolution
- Created a new Outlook profile
- Reconfigured the user’s email account
- Restarted Outlook
- Sync resumed successfully

## Verification
- New emails appeared in Outlook
- Send/Receive worked correctly
- User confirmed issue resolved

## Prevention / Notes
- Restart Outlook regularly if sync issues occur
- Use Outlook Web to confirm server-side status
- Recreate profile if sync problems persist

## Key Skills Demonstrated
- email troubleshooting
- Outlook diagnostics
- Microsoft 365 basics
- connectivity validation
- profile management
- root cause analysis
EOF