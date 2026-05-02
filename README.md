TERRITORY MANAGER - GOOGLE SHEETS INTEGRATION GUIDE					
					
STEP 1: PUBLISH THIS FILE TO GOOGLE SHEETS					
1. Upload this file to Google Drive					
2. Open it as Google Sheets (File > Open with > Google Sheets)					
3. The 4 sheets will be preserved: Territories, Assignments, Comments, README					
					
STEP 2: DEPLOY GOOGLE APPS SCRIPT (for write access)					
1. In Google Sheets, go to Extensions > Apps Script					
2. Paste the Apps Script code provided in the HTML app's Settings page					
3. Deploy as Web App: Execute as 'Me', Access 'Anyone'					
4. Copy the Web App URL					
					
STEP 3: CONFIGURE THE HTML APP					
1. Open the Territory Manager HTML file					
2. Go to Settings tab					
3. Paste the Apps Script Web App URL in 'Script URL' field					
4. Enter your Google Sheet ID (from the URL between /d/ and /edit)					
5. Enter your Google API Key (for read access from console.cloud.google.com)					
6. Tap 'Save & Connect', then tap the sync button (⟳) in the header					
					
SHEET STRUCTURE:					
Territories:	territory_id	last_completed_date			
Assignments:	assignment_id | territory_id | assigned_to | date_assigned | date_completed | service_year				
Comments:	comment_id | territory_id | assignment_id | comment_text | comment_date				
					
DATE FORMAT: YYYY-MM-DD (e.g., 2025-09-01)					
SERVICE YEAR FORMAT: YYYY-YYYY (e.g., 2024-2025, Sept to Aug)					
					
