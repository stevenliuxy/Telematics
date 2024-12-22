<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Telematics 1220</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__html"><p><strong>Version 2.1.0-alpha</strong> – Released on December 20, 2024</p>
<p>We’re excited to announce the release of Version 2.1.0-alpha! This update brings significant improvements to the user experience, including several new features, bug fixes, and performance enhancements.</p>
<h3 id="new-features">New Features:</h3>
<ul>
<li><strong>Refined Homepage dashboard</strong>: A redesigned dashboard with real-time data visualization and action-oriented insights for focused decision-making.
<ul>
<li><strong>Real-time asset status tracking</strong>: Monitors truck-battery pairs, showing real-time status (working, charging, idle, fault, offline).</li>
<li><strong>Optimization call-to-action</strong>:
<ul>
<li><em>Charging habits</em>: Identifies vehicles with over-discharging behavior and idle charging opportunities for improvement.</li>
<li><em>Utilization rates</em>: Flags high/low utilization vehicles, helping dealers assess purchase needs or offer operational improvements.</li>
</ul>
</li>
<li><strong>Battery health monitor</strong>: Alerts for abnormal battery usage and health degradation.</li>
<li><strong>Forklift fault tracking</strong>: Real-time (today) error codes for immediate issue resolution.</li>
</ul>
</li>
<li><strong>Enhanced Asset Management Center</strong>: A streamlined asset list with key details for quicker insights.
<ul>
<li><strong>Vehicle data center</strong>: All vehicle-related information in one place</li>
<li><strong>View by fleet</strong>: Organize assets and view statistics by sub-dealer or custom groups.</li>
<li><strong>Asset location</strong>: Location tracking on a map.</li>
</ul>
</li>
<li><strong>Enhanced Fault Management Center</strong>: Centralized view of error codes and battery issues.
<ul>
<li><strong>Forklift Faults</strong>: Real-time and historical error codes, with controller data and QuickSolution support. Displayed faults fall into one of the following categories (see table 1).</li>
<li><strong>Battery Alerts</strong>: Historical alerts for unhealthy battery behavior and issues. Displayed alerts fall into one of the following categories (see table 2).</li>
</ul>
</li>
<li><strong>Enhanced Maintenance Center</strong>: Simplified tracking of forklift maintenance schedules based on working hour.</li>
<li><strong>Account Roles &amp; Permissions</strong>: Role-based access control for secure data management (see table 3).</li>
<li><strong>Dark Mode</strong>: A new dark theme for improved usability in low-light environments.</li>
</ul>
<p><strong>Table 1</strong></p>

<table>
<thead>
<tr>
<th>Fault Type/Fault Level</th>
<th>S</th>
<th>A</th>
<th>B</th>
</tr>
</thead>
<tbody>
<tr>
<td>Master Traction</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>Slave Traction</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>Pump</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>EPS</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>Battery</td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table><p><strong>Table 2</strong></p>

<table>
<thead>
<tr>
<th>Alert Type/Alert Level</th>
<th>S</th>
<th>A</th>
<th>B</th>
</tr>
</thead>
<tbody>
<tr>
<td>During Working</td>
<td></td>
<td>Over-discharge</td>
<td>Over/under-voltage, over/under-temperature</td>
</tr>
<tr>
<td>During Charging</td>
<td></td>
<td>Over-temperature</td>
<td>Charging too frequent (charger fault)</td>
</tr>
<tr>
<td>Battery Health</td>
<td></td>
<td>SOH degradation</td>
<td>Large cell-level voltage difference</td>
</tr>
</tbody>
</table><p><strong>Table 3</strong></p>

<table>
<thead>
<tr>
<th>Access/Role</th>
<th>Internal–Admin</th>
<th>Internal–Support</th>
<th>Internal–Sales</th>
<th>Internal–Basic</th>
<th>External–Dealer admin</th>
<th>External–End-user admin</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Function Accesss</strong></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>Homepage</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
</tr>
<tr>
<td>Asset Mgmt (Data)</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
</tr>
<tr>
<td>Asset Mgmt (Adjust Param/Start-Stop)</td>
<td>Yes</td>
<td>Yes</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>Fault Center</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
</tr>
<tr>
<td>Maintenance Center</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
<td></td>
</tr>
<tr>
<td>Sub-account Mgmt (Assign Forklift)</td>
<td>Yes</td>
<td></td>
<td></td>
<td></td>
<td>Yes</td>
<td></td>
</tr>
<tr>
<td><strong>Data Accesss</strong></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>Forklift scope</td>
<td>All trucks under region</td>
<td>All trucks under region</td>
<td>Only related accounts</td>
<td>Assign upon account creation</td>
<td>All trucks under dealer account</td>
<td>All trucks under user account</td>
</tr>
</tbody>
</table><blockquote>
<p>Currently unsafe to open full and partial forklift controls (param adjust) to non-support team. China ENG team will modify and update.</p>
</blockquote>
<h3 id="improvements">Improvements:</h3>
<ul>
<li><strong>Data Accuracy</strong>: Refined algorithms for improved data reliability and availability.</li>
<li><strong>Faster Load Times</strong>: Enhanced backend performance for quicker page loads.</li>
<li><strong>UI Enhancements</strong>: Simplified navigation and dynamic asset list for a smoother user experience.</li>
<li><strong>Improved Translations</strong>: Expanded and refined language support for better accessibility.</li>
<li><strong>Legacy Portal Removal</strong>: Streamlined experience by deprecating the old portal.</li>
<li><strong>Updated Truck ID Logic</strong>: Truck IDs now display as “custom name/SN” (if a custom name is assigned), “SN/forklift model” (if no custom name), or “DIS/VIN” (if serial number is missing).</li>
<li><strong>Fault Drill-Down Helper</strong>: Zooms data panels +/- 24 hours around fault occurrences, with annotated timestamps for quicker troubleshooting.</li>
<li><strong>Batch Add for Group Management</strong>: New batch add feature for efficient bulk asset management.</li>
<li><strong>Enhanced Exporting</strong>: More flexible and robust export options for reports, with customizable formats and filters.</li>
</ul>
<h3 id="bug-fixes"><strong>Bug Fixes:</strong></h3>
<ul>
<li><strong>[Muhammad 12/16 #1] Fault Number Alignment in Vehicle Center</strong>: “Fault Type” chart now filters out non-S, A, and B-level error codes. Future versions will only display error codes with assigned priority levels.</li>
<li><strong>[Muhammad 12/16 #2] Vehicle Report Export</strong>: Export function added to all report items for improved reporting flexibility.</li>
<li><strong>[Muhammad 12/16 #3] Fault Count Calculation Error</strong>: Percentage change calculated as:
<ul>
<li><strong>Past 24 hrs</strong>: Today’s fault count vs. the 7-day average daily fault count.</li>
<li><strong>Last 7 days</strong>: Last 7-day fault count vs. previous 7-day.</li>
</ul>
</li>
<li><strong>[Muhammad 12/16 #4] Fault Center Fault Count Inconsistency</strong>: Unified the underlying data definition for consistency.</li>
<li><strong>[Muhammad 12/16 #5] Fault Center Page Refresh Issue</strong>: Resolved.</li>
<li><strong>[Muhammad 12/16 #6] Fleet Report Graph Missing</strong>: Resolved.</li>
<li><strong>[Muhammad 12/04 #1] Missing Data for First Date of Selected Time Horizon</strong>: Resolved.</li>
<li><strong>[Muhammad 12/04 #2] Missing Data for Latest Date</strong>: Data for dates within the selected range but not displayed is due to lagged-calculation for that specific date.</li>
<li><strong>[Muhammad 12/03 #1] Chinese Menu Items</strong>: Resolved.</li>
<li><strong>[Muhammad 12/03 #2] Export Function Update</strong>: Now supports exporting only selected trucks. All data tabs are included to avoid confusion. Since data table dimension may vary, a total column may not always be applicable and is therefore not included at this time.</li>
<li><strong>[Muhammad 12/03 #3] Map Display Error</strong>: Resolved.</li>
<li><strong>[Muhammad 12/03 #4] Asset List Button Duplication</strong>: Resolved.</li>
<li><strong>[Muhammad 12/03 #5] Start-Stop Translation Issue</strong>: Resolved.</li>
</ul>
<h3 id="known-issues">Known Issues:</h3>
<ul>
<li><strong>Data Delay</strong>: Except for live data, report statistics are calculated with a 1-day look-back window. Users may experience delays in data availability due to the scheduling gap between calculation points.</li>
<li><strong>Fault and Alert Reporting</strong>: Only ranked (S, A, B) error codes and alerts are reported. New error codes can be added to the list, and irrelevant or frequently occurring codes may be removed.</li>
</ul>
<h3 id="additional-notes"><strong>Additional Notes:</strong></h3>
<ul>
<li><strong>Next Release (December 31, 2024)</strong>: Includes new features:
<ul>
<li><strong>User SSO Login</strong></li>
<li><strong>Account Roles and Permissions Management</strong></li>
</ul>
</li>
<li><strong>Support Contact</strong>: For assistance, reach out to our team at <a href="mailto:zhuhaibin@ep-ep.com">zhuhaibin@ep-ep.com</a> and <a href="mailto:zhuhaibin@ep-ep.com">liuxiaoyu@ep-ep.com</a>.</li>
</ul>
</div>
</body>

</html>
