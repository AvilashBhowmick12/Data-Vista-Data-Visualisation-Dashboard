# [DATA VISTA DATA VISUALISATION DASHBOARD](https://github.com/AvilashBhowmick12/Data-Vista-Data-Visualisation-Dashboard) 
![Black Dashboard Flask - Admin Dashboard coded in Django.](https://github.com/AvilashBhowmick12/Data-Vista-Data-Visualisation-Dashboard/blob/main/media/datavistaloginpage.gif)

<br />

> Features:

- ✅ `Up-to-date dependencies`
- ✅ Black Dashboard, BS4 Design
- ✅ `DB Tools`: SQLAlchemy ORM, `Flask-Migrate` (schema migrations)
- ✅ `Persistence`: Azure(PostgreSQL) (prod)
- ✅ `Authentication`: Session Based, `OAuth` via Github / via Database(AZURE)
- ✅ `Deployment`: Docker, Page Compression (Flask-Minify) 


## Demo

- **Data Vista Dashboard Flask** [Login Page](https://github.com/AvilashBhowmick12/Data-Vista-Data-Visualisation-Dashboard/blob/main/media/datavistaloginpage.gif)

<br />

## Docker Support

> Get the code

```bash
$ git clone https://github.com/AvilashBhowmick12/Data-Vista-Data-Visualisation-Dashboard.git
$ cd Data-Vista-Data-Visualisation-Dashboard
```

> Start the app in Docker

```bash
$ docker-compose up --build 
```

Visit `http://127.0.0.1:5000/` in your browser. The app should be up & running. [only possible after running the python commands]

<br />

## Create/Edit `.env` file

The meaning of each variable can be found below: 

- `DEBUG`: if `True` the app runs in develoment mode
  - For production value `False` should be used
- `ASSETS_ROOT`: used in assets management
  - default value: `/static/assets`
- `OAuth` via Github
  - `GITHUB_ID`=<GITHUB_ID_HERE>
  - `GITHUB_SECRET`=<GITHUB_SECRET_HERE> 

<br />

## Manual Build

> UNZIP the sources or clone the private repository. After getting the code, open a terminal and navigate to the working directory, with product source code.

### 👉 Set Up for `Windows` 

> Install modules via `VENV` (windows) 

```
$ virtualenv env
$ .\env\Scripts\activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Flask Environment

```bash
$ # CMD 
$ set FLASK_APP=run.py
$ set FLASK_ENV=development
$
$ # Powershell
$ $env:FLASK_APP = ".\run.py"
$ $env:FLASK_ENV = "development"
```

<br />

> Start the app

```bash
$ flask run
// OR
$ flask run --cert=adhoc # For HTTPS server
```

At this point, the app runs at `http://127.0.0.1:5000/`. 

---

## Documentation

The documentation for the **Data Vista Dashboard Flask** is hosted at our [website](https://github.com/AvilashBhowmick12/Data-Vista-Data-Visualisation-Dashboard/tree/main/Documentation)

<br />

## File Structure -- Contributors in this project || NAMES MENTIONED || 

Within the download you'll find the following directories and files:

```bash
< PROJECT ROOT >
   |
   |-- apps/
   |    |
   |    |-- home/                           # A simple app that serve HTML files
   |    |    |-- routes.py                  # Define app routes | made changes for the routing by -- avilash and pranita
   |    |
   |    |-- authentication/                 # Handles auth routes (login and register)
   |    |    |-- routes.py                  # Define authentication routes  
   |    |    |-- models.py                  # Defines models  
   |    |    |-- forms.py                   # Define auth forms (login and register) 
   |    |
   |    |-- static/
   |    |    |-- <css, JS, images>          # CSS files, Javascripts files || made changes as per the graphs by Pranita
   |    |
   |    |-- templates/                      # Templates used to render pages
   |    |    |-- includes/                  # HTML chunks and components
   |    |    |    |-- navigation.html       # Top menu component || made by Pavan | modified by Avilash 
   |    |    |    |-- navigation-sales.html          # navigation header as per the sales page | made by ankit, | modified by Pranita
   |    |    |    |-- sidebar.html          # Sidebar component
   |    |    |    |-- footer.html           # App Footer
   |    |    |    |-- scripts.html          # Scripts common to all pages
   |    |    |
   |    |    |-- layouts/                   # Master pages
   |    |    |    |-- base-fullscreen.html  # Used by Authentication pages
   |    |    |    |-- base.html             # Used by common pages
   |    |    |
   |    |    |-- accounts/                  # Authentication pages
   |    |    |    |-- login.html            # Login page | linked with the Database and its routing and functionality by Avilash
   |    |    |    |-- register.html         # Register page by Avilash
   |    |    |
   |    |    |-- home/                      # UI Kit Pages
   |    |         |-- index-order-page-financial.html            # Index-order-page for financial || made by Malleswari and Balakumari
   |    |         |-- index-order-page-sales.html                # index-order page for the sales manager || MAde by Pujitha and Sirisha
   |    |         |-- index-data-metric-page-financial.html            # Index-data-metricr-page for financial || Made by Pranita
   |    |         |-- index-data-metric-page-sales.html               # index data metric for sales manager || made by Balakumari and Pradeep
   |    |         |-- index-product-page-financial.html            # Index-product-page for financial || made by Ritik , Accompanied by Dinakar
   |    |         |-- index-product-page-sales.html            # Index-product-page for sales || made by Prathiksha and satya || modified by Pranita
   |    |         |-- index-report-financial.html               # Last minute modifications and fixes by Ankit, Avilash, Mallweswari and Pranita 
   |    |         |-- index-report-sales.html                   # Last minute modifications and fixes by Ankit, Avilash, Mallweswari and Pranita 
   |    |         |-- 404-page.html         # 404 page
   |    |         |-- *.html                # All other pages
   |    |    
   |  config.py                             # Set up the app
   |    __init__.py                         # Initialize the app
   |
   |-- requirements.txt                     # App Dependencies
   |
   |-- .env                                 # Inject Configuration via Environment
   |-- run.py                               # Start the app - WSGI gateway || all names are mentioned of the contributors
   |
   |-- ************************************************************************
```

---

## Useful Links

- [More products](https://www.creative-tim.com/bootstrap-themes) from Creative Tim
- [Tutorials](https://www.youtube.com/channel/UCVyTG4sCw-rOvB9oHkzZD1w)
- [Freebies](https://www.creative-tim.com/bootstrap-themes/free) from Creative Tim
- [Affiliate Program](https://www.creative-tim.com/affiliates/new) (earn money)

<br />

## Social Media

- LinkedIn: <https://www.linkedin.com/in/avilash-bhowmick-497b24223>
- Facebook: <https://www.facebook.com/CreativeTim>
- Figma: <https://tiny.cc/Avilash_DesktopPortfolio>
- Instagram: <https://www.instagram.com/desole_triste_prince>

<br />

---
[Data Vista Dashboard](https://github.com/AvilashBhowmick12/Data-Vista-Data-Visualisation-Dashboard) - Made under the supervision and for internship purpose by [Infosys Springboard]
