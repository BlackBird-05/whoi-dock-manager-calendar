Problem Statement
WHOI requires a reservation software solution that can reserve, schedule, and track the usage of berths of varying lengths and for different periods of time.
UI/UX Features
The software will have to have a calendar shown to the user with the different berths availability. 
When the user selects a date, a pop up should be displayed allowing the user to input details for vessel name, length, operator, contact, work number, cell number, and email. The user should also be able to select the period to reserve the berth. The system should verify the vessel length does not exceed the berth length.
Tech Stack
Frontend: Vanilla HTML, tailwind css, and javascript

Database: PostgreSQL (utilizing the btree_gist extension for exclusion constraints on ranges).

Potential Problems:
When two users submit a request almost concurrently, one user must have an error message displayed and their request should be reversed. 
Users need email code to make a cancellation request.

Future Implementations:
If this project is to be taken further, a user authentication system can be added also using Supabase in order to verify user identity prior to registration and cancellation.

Another cancellation request verification system would be to use supabase’s smtp mail system to email a verification code in order to complete every cancellation request.
