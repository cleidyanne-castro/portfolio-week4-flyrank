# Cleidyanne Castro — AI & Data Portfolio

Personal portfolio showcasing my work across AI, data engineering, backend development, and cloud technologies.

## Live Feature

The portfolio includes one working dynamic feature: a contact form.

The form uses FormSubmit to receive visitor messages and forward them to my email.

### Data flow

Visitor → HTML form → FormSubmit → Email

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
└── week4-stack-rationale.md