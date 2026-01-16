# TodoBox Sites

Official landing page for [TodoBox](https://github.com/faizal2007/todobox) - A modern Flask-based personal task management application with secure authentication, API token support, and multi-database compatibility.

## About

This repository hosts the static website for TodoBox at [https://faizal2007.github.io/todobox-sites/](https://faizal2007.github.io/todobox-sites/)

## Latest Updates (January 2026)

✨ **NEWEST FEATURES (January 2026):**
- ✅ **Simple Todo Mode** - Quick-creation checklist todos with on-the-fly conversion between simple and advanced modes
- 🏆 **Achievement Modal** - Interactive modal for viewing completed todo details with time-to-completion tracking
- 🎯 **Smart Description Rendering** - Intelligent detection and rendering of markdown checklists vs advanced content
- 📊 **Dashboard Analytics** - Track tasks with donut charts grouped by time periods (today, weekly, monthly, yearly)
- 💡 **Wisdom Quotes** - Daily inspiration from ZenQuotes API with local fallback
- 📱 **PWA Support** - Install as a Progressive Web App on mobile and desktop devices

✨ **PREVIOUS UPDATES (2025):**
- 🔐 **Terms and Disclaimer Management** - Admin can create/manage terms with version control system
- 📝 **User Registration System** - Self-service registration with email verification and terms acceptance
- 🕐 **KIV Status** - Keep tasks in view with dedicated KIV (Keep In View) status for tasks on hold
- 🐛 **Critical Bug Fixes** - Mark as KIV button working, dashboard dates fixed, recent todos display corrected
- 🧪 **Comprehensive Testing** - Multi-layer testing strategy with 44+ tests covering backend, frontend, and assets
- 🔒 **Security Enhancements** - Account deletion cooldown, GitHub code scanning alerts addressed, pre-commit hooks
- ⚡ **Performance Optimization** - JavaScript modernization (jQuery to vanilla JS), 15% faster execution

## Features Highlighted

- 📝 **Todo Management** - Task organization with responsive grid layout, markdown support, and simple/advanced modes
- ✅ **Simple Todo Mode** - Quick checklist creation with on-the-fly conversion to advanced markdown editing
- 🏆 **Achievement Tracking** - View completed todos with detailed completion metrics and time tracking
- 💡 **Wisdom Quotes** - Daily inspiration from ZenQuotes API with local fallback quotes
- 👤 **User Authentication** - Email/password and Google OAuth sign-in with email verification
- 📋 **User Registration** - Self-service account creation with email verification and terms acceptance
- 🕐 **KIV Status** - Keep tasks in view with dedicated status for tasks on hold
- 📊 **Dashboard Analytics** - Task tracking with donut charts grouped by time periods (today, weekly, monthly, yearly)
- 🔑 **API Access** - RESTful API with Bearer token authentication for external integrations
- ⏰ **Smart Reminders** - Set reminders with automatic timezone detection and auto-close after 3 notifications
- 🌍 **Timezone Support** - Automatic timezone detection based on IP geolocation with 43+ timezone options
- 📱 **PWA Support** - Install as a Progressive Web App on mobile and desktop devices
- 🎨 **Modern UI** - Bootstrap 4 responsive design with loading indicators and smooth animations
- 🔒 **Security** - Password hashing, CSRF protection, XSS prevention, secure sessions, pre-commit hooks
- 💾 **Flexible Storage** - SQLite, MySQL, PostgreSQL support with migrations
- 📄 **Terms Management** - Admin-managed terms and disclaimer with version control
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

✅ **Production Ready** (January 2026 - Latest)

## Recent Updates (January 2026)

### Latest - New Features (January 2026)
- **Added**: Simple Todo Mode - Quick checklist creation with on-the-fly conversion between simple and advanced modes
- **Added**: Achievement Modal - Interactive modal for viewing completed todo details with time-to-completion tracking
- **Added**: Smart Description Rendering - Intelligent markdown checkbox detection and rendering
- **Added**: Dashboard Analytics - Donut charts grouped by time periods (today, weekly, monthly, yearly)
- **Added**: Wisdom Quotes - Daily inspiration from ZenQuotes API with local fallback
- **Added**: PWA Support - Install as a Progressive Web App on mobile and desktop devices

### Critical Fixes & Testing (2025)
- **Fixed**: Service Worker blocking external resources (CDN, fonts, scripts)
- **Fixed**: Recent Todos showing completed tasks and wrong page links
- **Fixed**: KIV todos not showing in KIV tab after marking, deletion foreign key errors
- **Added**: Comprehensive multi-layer testing (44+ tests: backend, frontend, assets)
- **Added**: Pre-commit hooks for quality assurance and syntax checking
- **Security**: Fixed GitHub code scanning alerts, account deletion cooldown system
- **Performance**: JavaScript optimization (jQuery to vanilla JS), 15% faster execution

### Previous Features (2025)
- **Added**: Terms and Disclaimer Management System with admin controls and version tracking
- **Added**: User Registration System with email verification and terms acceptance
- **Added**: KIV (Keep In View) status for tracking tasks on hold
- **Added**: Auto-close reminders after 3 notifications within 30 minutes
- **Added**: Timezone support with automatic detection and 43+ timezone options

### Previous Releases
- **v1.6.3** - Secure account deletion, root index route, PWA support
- **v1.6.0** - JavaScript optimization (jQuery to vanilla JS), 15% faster execution
- **v1.5.0** - Auto-close reminders, timezone support, PWA install
- **v1.4.0** - Dashboard time period grouping, reminder system
- **v1.3.3** - Reverse proxy support, OAuth fixes
- **v1.1.0** - API authentication with Bearer tokens

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