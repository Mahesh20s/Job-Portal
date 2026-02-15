# Job Portal

A Django-based job portal web application where employers can post jobs and job seekers can apply, bookmark jobs, and track applications.

## Features

- 👥 User authentication (job seekers & employers)
- 💼 Job posting & management (employers only)
- 📋 Job applications tracking
- ❤️ Job bookmarking/wishlist
- 🔍 Advanced filtering & search
- 📧 Email notifications
- 🌙 Dark mode support
- 📊 Dashboard with analytics

## Tech Stack

- **Backend**: Django 6.0
- **Database**: PostgreSQL (production) / SQLite (development)
- **Frontend**: HTML, CSS, JavaScript
- **Deployment**: Render/Heroku

## Local Setup

### Prerequisites
- Python 3.8+
- Git

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/YOUR_USERNAME/job_portal.git
cd job_portal
```

2. **Create virtual environment**
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Set up database**
```bash
python manage.py migrate
python manage.py populate_jobs  # Load sample data
```

5. **Create superuser (admin)**
```bash
python manage.py createsuperuser
```

6. **Run development server**
```bash
python manage.py runserver
```

Visit `http://localhost:8000` in your browser.

## Default Admin Setup

Once you create a superuser, access the admin panel at:
- URL: `http://localhost:8000/admin/`
- Add companies and jobs from the admin interface
- Or use the web interface at `/job/create/` (must be marked as employer)


   
  

## Project Structure

```
job_portal/
├── job_portal/          # Project settings
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── jobs/                # Main app
│   ├── models.py
│   ├── views.py
│   ├── forms.py
│   ├── templates/
│   ├── static/
│   └── migrations/
├── db.sqlite3
├── manage.py
└── requirements.txt
```

## Usage

### For Job Seekers
1. Register with email
2. Browse jobs with filters
3. Apply for positions
4. Track applications in dashboard
5. Bookmark favorite jobs

### For Employers
1. Register and check "I am an employer"
2. Post jobs via `/job/create/`
3. Edit/manage your listings
4. View applications in admin panel
5. Update application status

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is open source and available under the MIT License.

## Support

For issues or questions, please open an issue on GitHub.

## Author

Your Name - [LinkedIn](www.linkedin.com/in/smahesh9923)

---

**Live Demo**: [Your Deployed URL Here]

**GitHub**: https://github.com/Mahesh20s/job_portal


