# 🗄️ Database and Persistence

## 1. Current database status

No database or persistence mechanism is included in the repository. The HTML pages are static documents and do not store visitor records, course enrollments, login credentials, or carousel state beyond the temporary browser component state.

There are no:
- Database servers or client libraries.
- Tables, collections or schema definitions.
- ORM models.
- Migration scripts.
- API endpoints that read or write records.
- Backup or recovery jobs.

## 2. Form fields are not a database

Task 3 displays email and password input fields in a modal. The form has no action URL or event handler. Values are not intentionally sent to an application backend by the project code and are not stored by a project database.

Task 1's Enroll Now link is a placeholder. It does not create an enrollment record.

## 3. Static assets

Files in `media/` and `output/` are repository assets. They are not user records or application storage.

## 4. Future data-backed behavior

If this exercise is expanded into a real learning platform, the data design must be created before implementation. Requirements would include:
- User and role model.
- Course catalogue and enrollment lifecycle.
- Authentication and authorization model.
- Data minimization and privacy disclosures.
- Password hashing and session security, if password authentication is selected.
- Retention, deletion and export requirements.
- Backups, restoration testing, and access auditing.
- Secure migrations and least-privilege database access.

Do not publish an ERD or database schema as current architecture until a real schema exists.
