# To-Do List for PAS Intervention 2.0 Website and Email System

## Website Development Tasks

 1. **Create Website Structure and Branding**✅

    - Develop the website named "Physical Activity Self-efficacy (PAS) Intervention 2.0."
    - Restrict access to invited research participants only.
    - Implement researcher-editable text for all website content.

 2. **Implement Account Creation (Information 2)**✅

    - Create a registration page requiring:
      - Registration code: "wavepa" (non-case-sensitive).
      - Required fields: ID (non-case-sensitive), password (case-sensitive), password confirmation, email address (non-case-sensitive), phone number.
      - Optional field: Full Name.
    - Add password reset functionality on the login page.
    - Ensure accounts are not activated until email confirmation (see Information 3).

 3. **Set Up Email Confirmation (Information 3)**

    - Develop an email system to send a confirmation email immediately after registration.
    - Include a clickable link in the email to activate the account.
    - Allow researchers to edit the email template (subject: "Confirm to Activate Your Account") via the administration site.

 4. **Build Eligibility Interest Page (Information 4)**

    - Create a page post-account creation asking participants if they are interested in determining eligibility (1-2 minutes).
    - Include "Interested" and "Not Interested" buttons, with a text field for reasons if "Not Interested" is selected.
    - Ensure text is editable by researchers via the administration site.

 5. **Develop Eligibility Criteria Page (Information 5)**

    - Implement a form with the following questions:
      - Age (options: &lt;18, 19, …, 64, &gt;64; eligible: 18-64 years).
      - Height in inches (options: &lt;48, 48, …, 83, &gt;83) and weight in pounds (&lt;120, 120, …, 500, &gt;500) for BMI calculation (eligible: BMI ≥ 25.00).
      - Access to a technological device (Yes/No; eligible: Yes).
      - Agreement not to enroll in other research-based intervention programs (Yes/No; eligible: Yes).
      - Willingness to comply with physical activity monitoring instructions (Yes/No; eligible: Yes).
      - Willingness to respond to study-related contacts (Yes/No; eligible: Yes).
    - Direct eligible participants to the IRB Consent Form (Information 6) and ineligible participants to the Exit Screen (Information 7).

 6. **Create IRB Consent Form Page (Information 6)**

    - Display a consent form for eligible participants with "Consent to Participate" and "Decline Participation" buttons (fix text field for decline reason).
    - Set Day 1 as the date of clicking "Consent to Participate" for scheduling.
    - Direct consenting participants to the Waiting Screen (Information 8) and declining participants to the Exit Screen (Information 7).
    - Allow researchers to edit the form text via the administration site.

 7. **Implement Exit Screen (Information 7)**

    - Create a page for ineligible participants or those declining consent.
    - Include researcher-editable text and contact information for Seungmin Lee.
    - Ensure the page is displayed as specified in Information 5 and 6.

 8. **Develop Waiting Screen (Information 8)**

    - Create a persistent page for enrolled participants, displayed after consent unless updated by Information 11, 15, or 22.
    - Include researcher-editable text and contact information.

 9. **Build Wave 1 Physical Activity Code Entry Page (Information 11)**

    - Display a code entry field (code: "wavepa", non-case-sensitive) from Day 11 to Day 20.
    - Show an error message for incorrect code entries.
    - Remove the page on Day 21 (e.g., if enrolled on 01/01/2025, remove on 01/21/2025).
    - Trigger email (Information 12) upon correct code entry by Day 20.
    - Trigger email (Information 14) on Day 21 if no code is entered.
    - Allow researchers to edit text via the administration site.

10. **Implement Double-Blind Randomization (Information 15)**

    - On Day 29 at 7 AM CT, randomize participants into Group 0 (control, access post-Day 113) or Group 1 (intervention, access Days 29-56).
    - Track engagement (e.g., number of challenges completed) for Group 1 only.
    - Trigger emails (Information 16 for Group 0, Information 17 for Group 1) post-randomization.

11. **Create Wave 3 Physical Activity Code Entry Page (Information 22)**

    - Display a code entry field (code: "wavepa", non-case-sensitive) from Day 95 to Day 104.
    - Show an error message for incorrect code entries.
    - Remove the page on Day 105 (e.g., if enrolled on 01/01/2025, remove on 04/15/2025).
    - Trigger email (Information 23) upon correct code entry by Day 104.
    - Trigger email (Information 25) on Day 105 if no code is entered.
    - Allow researchers to edit text via the administration site.

## Email Automation Tasks

 1. **Wave 1 Online Survey Set Email (Information 9)**

    - Send on Day 1 after consent, copying Seungmin Lee (svu23@iastate.edu).
    - Include a survey link and consent document download link, editable by researchers.
    - Offer $5 Amazon gift card for completion within 10 days.
    - Explore sending via text message (discuss with researchers).
    - Allow text revisions via the administration site.

 2. **Wave 1 Physical Activity Monitoring Email (Information 10)**

    - Send on Day 11 at 7 AM CT, copying Seungmin Lee.
    - Notify participants to meet research members within 10 days for monitoring.
    - Offer $35 Amazon gift card for completion.
    - Explore sending via text message.
    - Allow text revisions via the administration site.

 3. **Physical Activity Monitoring Tomorrow Email (Wave 1, Information 12)**

    - Send immediately after correct code entry (Information 11), copying Seungmin Lee.
    - Instruct to wear monitor for 7 days starting tomorrow, with $35 gift card for 4+ days (including one weekend day, 10+ hours/day).
    - Explore sending via text message.
    - Allow text revisions via the administration site.

 4. **Survey and Monitor Return Email (Wave 1, Information 13)**

    - Send 8 days after code entry (e.g., code on 01/20/2025, send on 01/28/2025) at 7 AM CT, copying Seungmin Lee.
    - Include survey link and instructions to return monitor.
    - Explore sending via text message.
    - Allow text revisions via the administration site.

 5. **Missing Code Entry Email (Wave 1, Information 14)**

    - Send on Day 21 at 7 AM CT to participants who missed code entry, copying Seungmin Lee.
    - Notify of missed $35 gift card but continued study participation.
    - Explore sending via text message.
    - Allow text revisions via the administration site.

 6. **Intervention Access Later Email (Information 16)**

    - Send on Day 29 at 7 AM CT to Group 0, copying Seungmin Lee.
    - Notify of intervention access post-Day 113.
    - Explore sending via text message.
    - Allow text revisions via the administration site.

 7. **Intervention Access Immediately Email (Information 17)**

    - Send on Day 29 at 7 AM CT to Group 1, copying Seungmin Lee.
    - Provide immediate intervention access link and ID, with $20 gift card for 24+ challenges in 4 weeks.
    - Explore sending via text message.
    - Allow text revisions via the administration site.

 8. **Wave 2 Online Survey Set Email (Information 18)**

    - Send on Day 57 at 7 AM CT to all participants, copying Seungmin Lee.
    - Include survey link, offering $5 gift card for completion within 10 days.
    - Explore sending via text message.
    - Allow text revisions via the administration site.

 9. **No Wave 2 Physical Activity Monitoring Email (Information 19)**

    - Send on Day 67 at 7 AM CT to all participants, copying Seungmin Lee.
    - Notify no Wave 2 monitoring and upcoming tasks.
    - Explore sending via text message.
    - Allow text revisions via the administration site.

10. **Wave 3 Online Survey Set Email (Information 20)**

    - Send on Day 85 at 7 AM CT to all participants, copying Seungmin Lee.
    - Include survey link, offering $5 gift card for completion within 10 days.
    - Explore sending via text message.
    - Allow text revisions via the administration site.

11. **Wave 3 Physical Activity Monitoring Email (Information 21)**

    - Send on Day 95 at 7 AM CT to all participants, copying Seungmin Lee.
    - Notify to meet research members within 10 days for monitoring, offering $40 gift card.
    - Explore sending via text message.
    - Allow text revisions via the administration site.

12. **Physical Activity Monitoring Tomorrow Email (Wave 3, Information 23)**

    - Send immediately after correct code entry (Information 22), copying Seungmin Lee.
    - Instruct to wear monitor for 7 days starting tomorrow, with $40 gift card for 4+ days (including one weekend day, 10+ hours/day).
    - Explore sending via text message.
    - Allow text revisions via the administration site.

13. **Survey and Monitor Return Email (Study End, Information 24)**

    - Send 8 days after Wave 3 code entry (e.g., code on 04/14/2025, send on 04/22/2025) at 7 AM CT, copying Seungmin Lee.
    - Include survey link, monitor return instructions, and intervention access for Group 0.
    - Explore sending via text message.
    - Allow text revisions via the administration site.

14. **Missing Code Entry Email (Study End, Information 25)**

    - Send on Day 105 at 7 AM CT to participants who missed Wave 3 code entry, copying Seungmin Lee.
    - Notify of missed $40 gift card, study end, and intervention access.
    - Explore sending via text message.
    - Allow text revisions via the administration site.

## Data Management Tasks

1. **Enable Data Download (Information 26)**

   - Allow developers and researchers to download data for Information 2, 3, 4, 5, 6, 11, 15, and 22 from the administration site, preferably during the study.
   - Format data per "4. PAS data format_2.0 example.xlsx."

2. **Test Website on Compressed Schedule (Information 26)**

   - Enable testing of the website within a compressed schedule (e.g., 112 minutes instead of 112 days) per "2. timeline example_R0_final.xlsx."

## Additional Tasks

1. **Track Revisions**

   - Ensure all green-colored text revisions are trackable.
   - Allow slight modifications by developers while maintaining functionality.

2. **Discuss Text Message Integration**

   - Discuss feasibility of sending emails as text messages for Information 9, 10, 12, 13, 14, 16, 17, 18, 19, 20, 21, 23, 24, and 25 with researchers.

## Notes

- All emails must copy Seungmin Lee (svu23@iastate.edu) and accommodate additional email addresses in the future.
- Study ends on Day 112 from enrollment (Day 1).
- Ensure all website and email content is editable via the administration site.

- [ ] Prioritize tasks to meet the one-week deadline, focusing on critical functionalities like account creation, eligibility screening, and email automation.