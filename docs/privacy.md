# 🛡️ Privacy Considerations

## Current state

The task pages do not submit data to a project-owned backend and do not include analytics, application cookies, or database persistence. Task 3 presents email/password controls as a UI exercise only.

Do not ask visitors or students to enter real credentials into the modal. Do not describe the page as collecting or protecting account information.

## Third-party dependencies

The browser requests Bootstrap CSS and JavaScript from jsDelivr. Review external dependency behavior and applicable provider documentation before using the pages in a production context.

## Image rights and attribution

The media directory contains local image files, but the HTML does not record their authors or reuse licenses. Verify ownership and permitted redistribution before publication. The MIT source-code license does not automatically cover third-party media.

## If data collection is introduced

Before adding registration, contact, analytics, or login functionality:
1. Define the purpose and minimum set of data.
2. Publish a clear privacy notice.
3. Identify service providers and recipients.
4. Establish access controls and secure transport.
5. Define retention, deletion, and user-request processes.
6. Protect logs and backups.
7. Provide a process for privacy questions and incident response.

Update this document whenever a cookie, tracker, API, account, payment provider, form processor, or persistent store is introduced.
