# DateHelper
Simple date functionality tool to allow easy creation and manipulation of calendar dates according to different ruless.

Goal: Create a java service/library which can generate detailed schedules and calendars according to direct input, days-till, and every-x rules.

Rules: Has to be java based, has to be easily included in a project via xml, gradle, maven, and other similar tools. Dependencies must be pre-existing and trusted java or spring tools.

Description: Given a specific date, count, or Year/Month/Week/Day input, generate an accurate calendar that holds all dates up to 100 years forward from the current date. All data should be stored in a Calendar object which can be listened to by another service in order to drive updates to a database, website, or other application. The Calendar should update each time a user adds a new special date, or yearly upon iterating. A default Calendar should be Gregorian, and should not include any holidays. The Calendar should have functionality to allow updates to specific dates, create new rules based on time passed (ex: every 100 days), and create new rules based on generalized times (ex: every third Saturday of the month) or any combination of these (ex: Every third weekend for the next two years excluding Jan 7th 2023).