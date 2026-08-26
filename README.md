# Cleidyanne Castro | AI and Data Portfolio

Personal portfolio showcasing my work across AI, data engineering, backend development, and cloud technologies.

## Live Feature

The portfolio includes one working dynamic feature: a contact form.

The form uses FormSubmit to receive visitor messages and forward them to my email. The name, email address, and message are sent to that external service when the form is submitted.

### Data flow

Visitor -> HTML form -> FormSubmit -> email

The browser performs required field and email format validation before a request is sent. A status message appears while the request is being submitted.

## Technologies

- HTML
- CSS
- Git
- GitHub
- FormSubmit

## What I Learned

The portfolio itself is a static website, so it does not have its own backend.

For the contact form, I connected the HTML form to an external service instead of building a backend from scratch. When a visitor submits the form, the browser sends the form data to FormSubmit, which processes the submission and forwards it to my email.

This helped me understand the difference between a frontend, a backend, and an external service handling data.

## Project Structure

```text
anne-portfolio-week4/
├── index.html
├── README.md
├── EVIDENCE.md
├── fix-log.md
└── week4-stack-rationale.md

## Reproduce locally

```bash
python3 -m http.server 8000
```

Open `http://127.0.0.1:8000` and test the form with an invalid email, an empty required field, and a valid test message. A real delivery check requires access to the configured mailbox.

## Limitations

This repository does not contain a backend or a local delivery inbox. FormSubmit is a third-party dependency, so its availability, response page, and delivery are outside the repository.
