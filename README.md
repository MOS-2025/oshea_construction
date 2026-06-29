# O'Shea Construction Blog

## Overview

O'Shea Construction Blog is a Full-Stack web application developed using the Django framework. The application provides informative articles aimed at Irish homeowners planning building, renovation, maintenance, and home improvement projects.

The application allows authorised users to create, edit and manage blog content while visitors can browse informative construction articles through a responsive and user-friendly interface.

The project demonstrates a database-backed MVC application built using Python, Django, PostgreSQL, HTML, CSS and Bootstrap while following Agile software development practices.

## Live Project

**Live Site:** *( Heroku URL)*

**Repository:** *(GitHub Repository URL)*

---

# User Experience (UX)

## Target Audience

The website has been designed for:

- Irish homeowners
- Property owners planning renovations
- Customers seeking building advice
- Potential construction clients
- DIY enthusiasts

## User Stories

### Visitor

- As a visitor, I want to browse blog articles so that I can learn about construction topics.
- As a visitor, I want the website to be responsive so I can read articles on any device.
- As a visitor, I want articles to be easy to navigate.

### Registered User

- As a registered user, I want to log in securely.
- As a registered user, I want my login status to be visible.
- As a registered user, I want to interact with content where permitted.

### Administrator

- As an administrator, I want to create blog posts.
- As an administrator, I want to edit blog posts.
- As an administrator, I want to delete blog posts.
- As an administrator, I want to upload featured images.
- As an administrator, I want to manage website content efficiently.

---

# Agile Development

This project was planned using Agile methodology.

Development was broken into manageable User Stories which were completed over multiple iterations.

Typical User Stories included:

- Project setup
- Database creation
- Authentication
- CRUD functionality
- Deployment
- Testing
- Documentation

Each completed User Story was linked to the project board before implementation.

## Agile Board

Insert screenshot and link to GitHub Projects or Trello.

---

# Design

## Colour Scheme

The website uses neutral construction-inspired colours to create a professional appearance suitable for a building company.

*(Insert colour palette screenshot.)*

## Typography

The typography was selected to maximise readability across desktop and mobile devices.

*(Insert font details.)*

## Wireframes

Wireframes were produced during the planning stage for:

- Home Page
- Blog Listing
- Blog Detail
- Login
- Admin Interface

*(Insert wireframe images.)*

---

# Database Design

The project uses PostgreSQL as its relational database.

## Entity Relationship Diagram

*(Insert ER Diagram.)*

## Post Model

| Field | Type |
|--------|------|
| Title | CharField |
| Slug | SlugField |
| Author | ForeignKey |
| Featured Image | CloudinaryField |
| Content | TextField |
| Excerpt | TextField |
| Created On | DateTimeField |
| Updated On | DateTimeField |
| Status | IntegerField |

---

# Features

## Existing Features

### Responsive Layout

The application works across desktop, tablet and mobile devices.

---

### Navigation

Responsive navigation allows users to browse the website easily.

---

### Blog Listing

Displays all published construction articles.

---

### Blog Detail

Displays the selected article with its full content and featured image.

---

### Authentication

Users can securely:

- Register
- Log in
- Log out

---

### Django Admin

Administrators can manage website content through Django Admin.

---

### CRUD Functionality

Administrators can:

- Create blog posts
- Read blog posts
- Update blog posts
- Delete blog posts

---

### Rich Text Editing

Django Summernote provides formatted blog editing.

---

### Image Uploads

Cloudinary is used to host uploaded images.

---

### User Feedback

Users receive confirmation messages after successful actions.

---

# Future Features

Possible future improvements include:

- Search functionality
- Blog categories
- Tags
- Contact form
- Construction quotation request form
- User profiles
- Newsletter subscription
- Social media sharing
- Related posts
- Pagination improvements

---

# Technologies Used

## Languages

- HTML5
- CSS3
- JavaScript
- Python

## Frameworks

- Django
- Bootstrap 5

## Database

- PostgreSQL

## Libraries

- django-allauth
- django-crispy-forms
- crispy-bootstrap5
- django-summernote
- Cloudinary
- Gunicorn
- WhiteNoise

## Hosting

- Heroku

## Version Control

- Git
- GitHub

---

# Testing

## Manual Testing

| Feature | Expected Result | Result |
|----------|----------------|--------|
| Home page loads | Displays correctly | Pass |
| Blog listing | Posts displayed | Pass |
| Blog detail | Selected article displayed | Pass |
| Login | User authenticated | Pass |
| Logout | User logged out | Pass |
| Create post | Record created | Pass |
| Edit post | Record updated | Pass |
| Delete post | Record removed | Pass |
| Responsive layout | Works on mobile | Pass |

---

## HTML Validation

Custom HTML validated using the W3C HTML Validator.

*(Insert validation screenshots.)*

---

## CSS Validation

CSS validated using the W3C CSS Validator.

*(Insert screenshots.)*

---

## Python Validation

Python code validated using the CI Python Linter.

*(Insert screenshots.)*

---

## Lighthouse Testing

Google Lighthouse testing produced satisfactory scores for:

- Performance
- Accessibility
- Best Practices
- SEO

*(Insert Lighthouse screenshots.)*

---

## Browser Compatibility

The application was tested using:

- Google Chrome
- Firefox

---

# Bugs

## Fixed Bugs

- Cloudinary deployment configuration
- Template path issues
- Static files configuration
- Image rendering
- Deployment configuration

## Remaining Bugs

No known bugs at the time of submission.

---

# Deployment

The application was deployed using Heroku.

## Deployment Steps

1. Create a Heroku application.
2. Connect the GitHub repository.
3. Configure environment variables.
4. Add PostgreSQL database.
5. Configure Cloudinary.
6. Install Gunicorn.
7. Configure WhiteNoise.
8. Create a Procfile.
9. Set `DEBUG = False`.
10. Deploy the application.
11. Verify the deployed version matches local development.

---

# Local Development

## Clone Repository

```bash
git clone <repository-url>
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Create Environment Variables

Create a `.env` file containing:

```text
SECRET_KEY=
DATABASE_URL=
CLOUDINARY_URL=
```

## Apply Migrations

```bash
python manage.py migrate
```

## Run the Development Server

```bash
python manage.py runserver
```

---

# Security

Security measures implemented include:

- Environment variables for secret keys.
- Sensitive files excluded via `.gitignore`.
- `DEBUG = False` in production.
- Django authentication.
- Role-based permissions.
- Secure database credentials.

---

# Credits

## Content

Construction articles were researched and written specifically for this project with a focus on Irish homeowners and residential construction.

## Resources

- Django Documentation
- Bootstrap Documentation
- Heroku Documentation
- Cloudinary Documentation
- PostgreSQL Documentation
- Code Institute Learning Platform
- Stack Overflow

## Acknowledgements

Special thanks to:

- Code Institute
- My mentor
- My wife and childern for their support and patience while completing this project
