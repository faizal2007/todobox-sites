# TodoBox Sites

Official landing page for [TodoBox](https://github.com/faizal2007/todobox) - A modern Flask-based personal task management application with secure authentication, API token support, and multi-database compatibility.

## About

This repository hosts the static website for TodoBox at [https://faizal2007.github.io/todobox-sites/](https://faizal2007.github.io/todobox-sites/)

## Latest Updates (v1.6.3+ - Dec 7, 2025)

✨ **LATEST FIXES & IMPROVEMENTS:**
- 🐛 **Critical Bug Fixes** - Mark as KIV button working, dashboard dates fixed, recent todos display corrected
- 🧪 **Comprehensive Testing** - 25-test suite against real MySQL database, test files reorganized to tests/ folder
- 📝 **Markdown Standards** - Language specifiers added to all 354 code blocks across documentation
- 📚 **Documentation Cleanup** - Simplified CHANGELOG, reorganized docs structure, improved navigation
- 🔒 **Security Enhancements** - GitHub code scanning alerts addressed, debug mode disabled, CDN integrity checks
- 🗂️ **Better Organization** - Test structure follows Python best practices, all tests in tests/ folder

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

✅ **Production Ready** (December 7, 2025 - Latest)

## Recent Updates (December 7, 2025)

### Latest - Critical Fixes & Testing
- **Fixed**: Mark as KIV button not working on /undone page - updated route to add todo to KIV table
- **Fixed**: Dashboard dates showing as script tags - refactored momentjs to server-side Python datetime
- **Fixed**: Dashboard Recent Todos not displaying dates - simplified query with proper filtering
- **Added**: Comprehensive test suite (25 tests) against real MySQL database with 100% pass rate
- **Changed**: Test files reorganized to tests/ folder following Python best practices
- **Changed**: Documentation reorganized with simplified CHANGELOG and archived analysis docs

### Documentation & Standards (Dec 7)
- **Refactor**: Added language specifiers to all 354 bare code blocks in 24 markdown files
- **Improved**: Markdown compliance across all documentation with proper code fences
- **Security**: Fixed GitHub code scanning alerts (debug mode, CDN integrity checks)

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