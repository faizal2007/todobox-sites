# TodoBox Sites

Official landing page for [TodoBox](https://github.com/faizal2007/todobox) - A modern Flask-based personal task management application with secure authentication, API token support, and multi-database compatibility.

## About

This repository hosts the static website for TodoBox at [https://faizal2007.github.io/todobox-sites/](https://faizal2007.github.io/todobox-sites/)

## Latest Features (v1.3.5 - Nov 30, 2025)

✨ **NEW & UPDATED:**
- 🔑 **API Token Authentication** - Secure token-based API access for external integrations
- 🌐 **Reverse Proxy Support** - Werkzeug ProxyFix middleware for Nginx/SSH tunnel deployments
- ⚡ **Loading Indicators** - Visual feedback during async todo operations
- 📊 **Dashboard Improvements** - Recent todos view excludes completed items
- 🔒 **Enhanced Security** - Username immutability, secure API token management
- 📚 **Complete Documentation** - 23 comprehensive guides with 100+ code examples and accessibility compliance

## Features Highlighted

- 📝 **Todo Management** - Task organization with responsive grid layout and markdown support
- 👤 **User Authentication** - Email/password and Google OAuth sign-in
- 🔑 **API Access** - RESTful API with Bearer token authentication for external integrations
- 🎨 **Modern UI** - Bootstrap 4 responsive design with loading indicators
- 🔒 **Security** - Password hashing, CSRF protection, XSS prevention, secure sessions
- 💾 **Flexible Storage** - SQLite, MySQL, PostgreSQL support with migrations
- 🌐 **Reverse Proxy Ready** - Deploy behind Nginx with automatic proxy header handling
- 🚀 **Production Ready** - Gunicorn support, Werkzeug 3.0 compatibility, comprehensive deployment guides

## Technology Stack

- **Framework:** Flask 2.3.2 with Flask-Login 0.6.3
- **Database:** SQLAlchemy 1.4.17 (SQLite, MySQL, PostgreSQL)
- **Authentication:** Google OAuth with Bearer token API auth
- **Security:** Bleach 6.3.0 (XSS), Werkzeug 3.0.6 (hashing), Flask-WTF 1.2.2 (CSRF)
- **Migrations:** Flask-Migrate 4.1.0 with Alembic
- **Frontend:** Bootstrap 4, Jinja2, moment.js
- **Production Server:** Gunicorn 23.0.0 with ProxyFix
- **Python:** 3.10+

## Links

- **Main Repository:** [faizal2007/todobox](https://github.com/faizal2007/todobox)
- **Documentation:** [TodoBox Docs](https://github.com/faizal2007/todobox/tree/master/docs)
- **Changelog:** [CHANGELOG.md](https://github.com/faizal2007/todobox/blob/master/CHANGELOG.md)
- **API Reference:** [API.md](https://github.com/faizal2007/todobox/blob/master/docs/API.md)
- **Deployment Guide:** [DEPLOYMENT.md](https://github.com/faizal2007/todobox/blob/master/docs/DEPLOYMENT.md)

## Status

✅ **Production Ready** (November 30, 2025 - v1.3.5)

## Recent Releases

### v1.3.5 (Nov 30) - Documentation Recheck & Accessibility
- Fixed trailing punctuation in headings for markdown compliance
- Corrected emphasis usage in documentation files
- Enhanced accessibility standards compliance
- 23 comprehensive documentation files fully validated
- Complete documentation ecosystem with navigation guides

### v1.3.4 (Nov 29) - Documentation Update
- Fixed markdown formatting across all documentation files
- Updated code fence syntax for consistency
- All documentation now passes validation

### v1.3.3 (Nov 29) - Reverse Proxy Support & Dashboard Fix
- Werkzeug ProxyFix middleware for reverse proxy deployments
- OAuth callback URL support behind proxies
- Dashboard "Recent Todos" now excludes completed items
- Optimized query performance

### v1.3.2 (Nov 27) - UI/UX Enhancements
- Loading indicators for AJAX operations
- Button state management to prevent double-clicks
- Username immutability for security
- Enhanced user experience flow

### v1.1.0 (Nov 26) - API Authentication
- Bearer token-based API authentication system
- API token generation and management
- Secure external integrations
- JSON error responses for API requests

## Get Started

```bash
# Clone repository
git clone https://github.com/faizal2007/todobox.git
cd todobox

# Install dependencies
pip install -r requirements.txt

# Configure environment
cp .flaskenv.example .flaskenv
nano .flaskenv  # Edit with your settings

# Initialize database and create user
flask db upgrade
python3 create_user.py

# Run development server
flask run

# For production
gunicorn -w 4 -b 0.0.0.0:5000 todobox:app
```

## Documentation

**23 comprehensive guides** available in `/docs` with 100+ code examples:

### Getting Started
- **SETUP.md** - Installation and configuration for SQLite, MySQL, PostgreSQL
- **QUICKSTART.md** - Quick reference guide with commands
- **USER_CREATION.md** - First-time user setup and management

### API & Technical Reference
- **API.md** - Complete API reference with all endpoints
- **MODELS.md** - Database schema and entity relationships
- **ARCHITECTURE.md** - System design, patterns, and configuration

### Deployment & Operations
- **DEPLOYMENT.md** - Production deployment guide
- **DEPLOYMENT_CHECKLIST.md** - Pre-deployment verification
- **OAUTH_SETUP.md** - Google OAuth2 configuration

### Quality & Security
- **CODE_REVIEW.md** - Code quality analysis and fixes
- **SECURITY_PATCHES.md** - Security improvements documentation
- **WERKZEUG_FIX.md** - Werkzeug 3.0.6 compatibility

### Navigation & Index
- **DOCUMENTATION_MASTER_INDEX.md** - Complete documentation index
- **INDEX.md** - Documentation summary and quick navigation
- **OVERVIEW.md** - Project overview and features

### Additional Resources
- **PROGRESS_NOVEMBER_2025.md** - Latest session progress
- **Migration guides** - Database migration documentation
- Plus 8+ additional technical guides

## License

MIT License - see the [LICENSE](LICENSE) file for details.