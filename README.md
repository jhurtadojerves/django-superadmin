Superadmin
=====

Superadmin is a Django app based in django admin to build admin sites quickly and easily, and generate site page like django admin.

Detailed documentation is in the "docs" directory.

Quick start
-----------

1. Add "superadmin" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'superadmin',
    ]

3. Run ``python manage.py migrate`` to create the superadmin migrations.

4. Continue

Release process
---------------

### Required GitHub secrets

| Secret | How to get it | Where to configure |
|---|---|---|
| `PYPI_API_TOKEN` | pypi.org → Account Settings → API tokens → Add API token (scope: project `django-superadmin`) | GitHub → Settings → Secrets and variables → Actions → New repository secret |

### How to publish a new release

1. Go to GitHub → Releases → **Draft a new release**
2. Create a new tag with the format `vX.Y.Z` (e.g. `v1.2.8`)
3. Fill in the title and description
4. Click **Publish release** — the Action triggers automatically and uploads the package to PyPI

> The package version is derived from the release tag via `setuptools-scm`. No files need to be edited before releasing.