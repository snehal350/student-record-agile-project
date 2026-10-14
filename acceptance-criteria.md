# Acceptance Criteria

Acceptance criteria define observable conditions for accepting a user story. The criteria below are proposed examples.

## US-01 — Add student
- Required fields such as student ID and name are validated.
- A duplicate student ID is rejected with a clear message.
- A valid record is saved and can be retrieved.
- Invalid input does not create a partial record.

## US-02 — Search student
- An authorized user can search by student ID or name.
- Matching records are displayed clearly.
- A no-results message appears when no record matches.
- Unauthorized users cannot access restricted student details.

## US-05 — Add course
- Course code, title, and required details are validated.
- Duplicate course codes are rejected.
- A saved course appears in the course list.
- Validation errors explain what needs correction.

## US-09 — Record attendance
- Faculty can select a course and lecture date.
- Faculty can mark attendance for enrolled students.
- Attendance is saved against the correct course and date.
- The saved record can be viewed again.
- The system prevents accidental duplicate attendance entries for the same student, course, and session, or clearly supports an authorized correction.

## US-12 — Enter marks
- Faculty can select the relevant course and assessment.
- Marks must be within the configured valid range.
- Invalid values are rejected with a clear message.
- Saved marks are associated with the correct student and assessment.
- Changes are limited to authorized users.

## US-14 — Calculate grades
- Grade calculation follows institution-approved grading rules.
- Boundary values are handled consistently.
- The system displays the calculated grade with the source marks.
- Test cases cover minimum, maximum, and grade-boundary values.

## US-16 — Login
- The login page loads successfully.
- Registered users with valid credentials can log in.
- Invalid credentials display an appropriate error.
- Successful login opens the correct authorized landing page.
- Session handling prevents protected pages from being accessed without authentication.

## US-19 — Role-based access
- Each account is assigned an approved role.
- Users can access only the functions allowed by their role.
- Direct attempts to access restricted actions are denied.
- Permission changes take effect according to the session/security design.

## US-11 — Attendance report
- An authorized user can choose a course and date range.
- The report includes the matching attendance records.
- Empty results are handled clearly.
- Report totals are consistent with the underlying records.

## General acceptance checklist
- Requirements are testable and unambiguous.
- Validation and error messages are understandable.
- Access controls are checked.
- Relevant test results are recorded.
- Documentation is updated.
