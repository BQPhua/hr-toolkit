# HR Toolkit

A single-file internal HR tool (`index.html`) with no backend and no external dependencies.

## Modules
1. **Entitlements**: length of service, pro-rated annual leave and balance, sick/hospitalisation/maternity/paternity leave, notice period, indemnity in lieu of notice, and termination benefits (Employment Act 1955, as amended 2022).
2. **Overtime**: normal-day, rest-day and public-holiday OT for monthly-rated staff, with warnings for the RM4,000 threshold and the 104-hour monthly limit.
3. **Working days**: counts working days between two dates and adds N working days to a date. You can set the weekend (including Kedah/Kelantan/Terengganu) and edit the holiday list.
4. **Onboarding**: a tracker for new hires with a 20-task checklist (pre-boarding → probation confirmation), due dates, overdue flags, search/filter, print, and JSON/CSV export and import.

## Hosting (pick one)
- **Intranet / IIS / Apache / Nginx**: copy `index.html` into any web folder.
- **SharePoint**: upload to a document library. If it downloads instead of opening, host it on a web server or Azure Static Web Apps.
- **GitHub Pages / Netlify / Azure Static Web Apps**: drag and drop the folder.
- **Local**: double-click `index.html`.

## Notes
- Data (onboarding records, holiday list, theme) is saved in each user's browser (localStorage). It is not shared between users, so use Export/Import to back it up or move it.
- The sample holiday list only includes fixed-date national holidays. Add the lunar, Islamic and state holidays from the official gazette.
- All figures are statutory minimums and estimates, not legal advice.
- To customise the onboarding checklist, edit the `TEMPLATE` array in the script.
