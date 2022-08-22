<p align="center">
<img src="https://datasciience-ensiie.github.io/assets/img/logo_DS_transparent_alt.png" width="150"/>
</p>

<img src="https://img.shields.io/static/v1?label=DataScIIEnce&message=Associative project&color=007bff"/>&nbsp;&nbsp;<img src="https://img.shields.io/static/v1?label=Languages&message=HTML, CSS, JS (JQuery)&color=ff0000"/>&nbsp;&nbsp;<img src="https://img.shields.io/static/v1?label=Restriction&message=Open to public&color=26c601"/>


# DataScIIEnce WEBAPP V2

## Introduction

This Git repository is centralizing all the resources of the current website of **DataScIIEnce**.


## Instructions

**Prequisities** : Please make sure you have :
1. an active (non-deprecated Python version) $\longrightarrow$ `python3 -V`
2. an active version of **pip** package manager $\longrightarrow$ `pip3 --version`
3. the dependencies of this project $\longrightarrow$ `pip3 -r requirements.txt`


- Open a new testing (ASGI) server to check the update on web app 
```console
mkdocs serve
```

- Deploy on production server[^1]
```console
mkdocs gh-deploy
```
[^1]: The user needs the explicit rights to push on the prod. server. Otherwise, no action can be performed without the explicit authorization from the *Head of IT Systems*.


- If you want to create a new page hosted following the pattern: [https://datasciience-ensiie.github.io/page_name](https://datasciience-ensiie.github.io/page_name), you have to 
    - Create a document named `page_name.md` __inside__ the `docs/` folder
    - Add a **new line** inside the `mkdocs.yml` file, under the `nav` section :  
```
nav:    
  - New page: "../page_name"
```

Finally, we have :
```
nav:
  - Home: "../"
  - About: "../about"
  - Getting started: "../getting-started"
  - Sessions: "../sessions"
  - Conferences: "../conferences"
  - References: "../references"
  - Useful links: "../links"
  - Contact: "../contact"
  - License: "../license"
  - New page: "../page_name"
```

**DO NOT FORGET TO COMMIT/PUSH ON THE GIT REPOSITORY ANY MODIFICATIONS**

## License & Authors

- Development start date : Aug. 2022

Copyright &copy; 2022 DataScIIEnce. All rights reserved.

- Initial development & Maintener
    - Check the [AUTHORS.md](AUTHORS.md) for the authors details
- Other resources : all rights to respective authors