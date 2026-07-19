# 00-06 Project Folder Structure

## 1. Introduction

This document defines the internal folder structure of the LifeChronicle project. It explains how source code, templates, static resources, media, documentation, tools, and configuration files are organized within the project.

A consistent folder organization improves maintainability, simplifies navigation, and supports long-term scalability.

---

# 2. Folder Organization Philosophy

The folder structure is designed around the following principles:

* Modular development

* Separation of concerns

* Easy navigation

* Reusability

* Documentation-first development

* Future scalability

---

# 3. High-Level Folder Structure

```text

LifeChronicle/

│

├── apps/

├── config/

├── docs/

├── master_data/

├── requirements/

├── deployment/

├── tools/

├── tests/

├── templates/

├── static/

├── media/

├── logs/

├── backups/

└── manage.py
```

---

# 4. Django Application Structure

Each application follows a consistent structure.

```text

app_name/
│

├── admin.py

├── apps.py

├── models.py

├── urls.py

├── views.py

├── forms.py

├── services.py

├── validators.py

├── permissions.py

├── managers.py

├── signals.py

├── tests/

├── migrations/

├── templates/

├── static/

└── management/
```

Additional files are added only when required.

---

# 5. Documentation Organization

All documentation resides under the **docs** directory and is organized into numbered modules.

Documentation is version controlled and considered part of the project's source.

---

# 6. Static and Media Organization

Static resources contain application assets.

Media stores user-uploaded content.

User uploads are never committed to version control.

---

# 7. Development Resources

Developer utilities, automation scripts, master data, deployment resources, and test suites are maintained in dedicated directories outside business modules.

---

# 8. Folder Naming Standards

* Lowercase names

* Meaningful names

* Underscore separated where applicable

* Consistent naming throughout the project

---

# 9. Summary

The project folder structure provides a standardized, scalable, and maintainable organization for all project resources.

---

# 10. Next Document

**00-07 Development Environment Setup**
