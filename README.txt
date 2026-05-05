Electrician App - User Guide
====================================
Version: 2.0.0

Welcome to the Automating Innovating AI Electrician App — a streamlined, secure, and intuitive tool 
for managing production workflows, employee payroll, material usage, inventory, purchase orders, and data exports.

This version includes full RBAC (Role-Based Access Control) and subscription plan enforcement.

RBAC & PLAN ENFORCEMENT (NEW)
------------------------------
The application now includes centralized RBAC and plan-based feature access:

• Role-Based Access Control (RBAC)
  - Every module checks the logged-in user’s role before granting access.
  - Roles include:
      • Global Admin
      • Local Admin
      • Payroll Manager
      • Inventory Manager
      • PO Manager
      • Read-Only User
  - Unauthorized users are blocked from restricted modules.

• Subscription Plan Enforcement
  - Features are unlocked based on your subscription tier:
      • BASIC — Limited access (view-only payroll, basic admin tools)
      • PRO — Full payroll, job entry, materials, and PO creation
      • ENTERPRISE — All features including:
            - Auto payroll export
            - Inventory transactions
            - Purchase order PDF generation
            - Advanced reporting
  - If a user attempts to access a feature outside their plan, the app will redirect them to the Start Page.

• Session Verification
  - All sensitive modules require an active, verified session.
  - Sessions expire on logout or exit.

Key Features
------------
• Secure Login:
  - Encrypted password protection with industry-standard hashing.
  - RBAC-based access to all modules.

• Payroll Management:
  - Input and calculate weekly payroll with precision.
  - Calculate electrical material usage using:
      • Quantity × Pay Rate (e.g., 120 ft NM-B × $0.12/ft)
      • Per-piece rates (e.g., 15 receptacles × $3.50)
      • Hourly wage (e.g., 10 hours × $22.00)
      • Enter 0 in any quantity or rate field that does not apply
  - Add up to four employees for each job.
  - Automatic pay splitting among listed employees.
  - Payroll module requires PRO or ENTERPRISE plan.

• Employee Job Entry:
  Each job entry will require:
      - First and last name of each employee
      - Employee ID (if applicable)
      - Work hours and job roles
      - Builder, job site, model, and lot/block details
      - Optional: Electrical material info such as:
        • Cable types (e.g., NM-B 12/2, MC 12/2)
        • Devices (e.g., TR receptacles, switches, GFCI/AFCI)
        • Lighting (e.g., LED cans, disc lights)
        • Conduit and fittings (e.g., EMT, couplings, straps)
  - Requires PRO or ENTERPRISE plan.

• Pay Week Entry & Auto Export
  This application streamlines the process of marking pay cycles and exporting enhanced Excel reports.
  • Set the start and end day of the payroll period using a fullscreen interface.
  - Example: Start Day = Thursday, End Day = Wednesday
  - Payroll is exported automatically 2 days after the end day
  - Press Esc to exit fullscreen mode at any time

  • Authorization Required
  - Only verified sessions with proper RBAC permissions can access this module.
  - Requires PRO or ENTERPRISE plan.

  • What Gets Exported
  - Weekly employee payroll grouped by name or ID
  - Exported to Excel files saved monthly under:
    Documents/AIAI_PM_App/Payroll_Excels/YYYY-MM/Payroll_YYYY-MM.xlsx
  - Each employee gets a dedicated sheet labeled by week number
  - Totals are auto-calculated

  • After export:
  - You’ll be asked if you’d like to open the workbook immediately
  - Excel must be installed to view reports

  Tip: Ensure pay data is complete before the scheduled export date (End Day + 2).

• Material & Inventory Management:
  - Add, edit, and track electrical materials.
  - Manage supplier info, SKUs, cost, and reorder levels.
  - Automatic inventory deduction based on daily work entries.
  - Inventory updates require PRO or ENTERPRISE plan.
  - Inventory receiving requires ENTERPRISE plan.

• Purchase Orders (POs):
  - Generate purchase orders by supplier.
  - Add material items and quantities.
  - Save POs to the database.
  - Generate PDF purchase orders (ENTERPRISE only).
  - Receive PO items into inventory (ENTERPRISE only).
  - All PO modules require PO Manager role.

• Reporting:
  - Clean Excel-compatible CSV exports grouped by month/day.
  - Ability to customize export file names.
  - Some reports require ENTERPRISE plan.

• Auto-Updating:
  - Automatically checks for new app versions.

• Friendly Interface:
  - Designed for ease of use—no technical knowledge required!

System Requirements
-------------------
• Operating System: Windows 10 or later is required.
• Microsoft Excel must be installed to view reports.
• At least 900 MB of available local disk space is recommended:
    - Data is stored using the client's SQL Server Express Database.
    - Monthly Excel files are created with worksheets by day.

License Activation
------------------
This app requires a valid Gumroad license key to unlock full functionality.
• You will be prompted to enter your license key on first launch.
• The app verifies your key securely via Gumroad’s API.
• If the license is invalid or revoked, access will be restricted.
Note: Internet access is required for initial license validation.

Getting Started
---------------
1. Launch the app via the Electrician App icon.
2. Click 'Admin Registration' to create an account.
3. After registering, click 'Admin Login' to sign in.
4. Navigate to the Admin Interface.
5. Access modules based on your RBAC role and subscription plan.

Navigation & Exiting
---------------------
• Use the dashboard to access key modules.
• Click the 'Exit' button on any screen to close the app.

Tips
----
• Export data regularly to back up your records.
• Use strong admin credentials.
• Keep Excel updated for full report compatibility.
• Ensure your subscription plan matches your workflow needs.

Troubleshooting
---------------
• App won’t launch: Ensure Windows 10+ is installed and Excel is available.
• License key rejected: Double-check your Gumroad purchase email.
• Export failed: Confirm pay data is complete and Excel is installed.
• Access denied: Check your RBAC role and subscription plan.
• Auto-update not working: Check your internet connection and firewall settings.

Support
-------
Questions or feedback? Contact the developer:
automatinginnovatingai@outlook.com

Thank you for using Electrician App!
