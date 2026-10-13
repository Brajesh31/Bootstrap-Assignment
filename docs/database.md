# Data and persistence

## Database

There is no database or persistence layer in this project. The pages do not read or write user records, courses, enrollments, or credentials. There are no server-side models, migration files, or database connection settings.

## Form controls and sample content

Task_3.html contains email and password fields inside a modal for a visual UI example. The form does not submit data and has no authentication handler. Task_1.html shows sample course copy, but its action link is a placeholder and does not create an enrollment. The pages do not persist information between visits.

## Static assets

Images referenced by the HTML pages live in Assignment_14_Bootstrap/media/. The output folder stores example renders. Neither directory is an application data store. The images' provenance and distribution terms are not recorded in the HTML.

## Future data-backed behavior

If the project grows to accept real registrations or credentials, design an appropriate server-side service, storage schema, access control, retention and deletion rules, and secure transport before collecting information. Never store secrets in the static pages or in .env.example. Review the license and privacy terms for any dataset or media before distributing it.
