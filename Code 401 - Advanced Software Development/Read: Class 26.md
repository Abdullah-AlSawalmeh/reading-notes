# About Django

- Django is a high-level Python web framework that enables rapid development of secure and maintainable websites
- With Django, you can take Web applications from concept to launch in a matter of hours. Django takes care of much of the hassle of Web development, so you can focus on writing your app without needing to reinvent the wheel. It’s free and open source.

<img src="https://fiverr-res.cloudinary.com/images/q_auto,f_auto/gigs/148539243/original/1e851d0838d750357906c41b58eadf2f3b6364ec/make-your-python-django-project-with-postgresql.jpg" width="900px" height="400px">

## Installing an official release with pip

This is the recommended way to install Django.

Install pip. The easiest is to use the standalone pip installer. If your distribution already has pip installed, you might need to update it if it’s outdated. If it’s outdated, you’ll know because installation won’t work.
After you’ve created and activated a virtual environment, enter the command:

```
python -m pip install Django
```

### URLs and views

- A clean, elegant URL scheme is an important detail in a high-quality Web application. Django encourages beautiful URL design and doesn’t put any cruft in URLs, like .php or .asp.

-To design URLs for an application, you create a Python module called a URLconf. Like a table of contents for your app, it contains a simple mapping between URL patterns and your views.

```
from django.urls import path

from . import views

urlpatterns = [
    path('bands/', views.band_listing, name='band-list'),
    path('bands/<int:band_id>/', views.band_detail, name='band-detail'),
    path('bands/search/', views.band_search, name='band-search'),
]
```

## How Django Works Behind the Scenes

- Django is a Python-based web framework used by millions of developers and billions of consumers through popular apps like Instagram. It is open source, meaning the code is available for free on Github and can be downloaded onto any developer’s computer and used alongside the official documentation.

ِAlmost all popular open source packages have some degree of funding involved, typically in one of three forms:

1. Corporate Sponsor - A group of engineers within a larger, for-profit company decide to open-source internal code. This is how React (Facebook) and Angular (Google) emerged. Typically engineers at the company are paid, in part, to work on open source though community involvement from developers outside of the core company occurs as well. While this structure has the stability of a wealthy benefactor, there can be confusion around the licensing aspects at times.

2. Solo - An individual developer initially creates code, open sources it, and retains default control. This is the case for VueJS, Tailwind CSS, and Laravel, among others. Typically the lead developer either raises contributions directly like Evan You of VueJS, offer add-on services like Spark for Laravel, or the founders provide highly-paid consulting services.

3. Non-profit - This was Django’s approach early on, in 2008, when the Django Software Foundation was formed to promote, support, and advance Django.
