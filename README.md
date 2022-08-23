# template-wordpress-default
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->
Stackspot :: Default template for [Stack Wordpress](https://github.com/TheFirstSquad/stack-wordpress)

## Overview
The **template-wordpress-default** template adds to a stack the ability to provision the Wordpress development environment with a Docker container.

## Prerequisites
To use this template you need to use the `CLI` of `StackSpot` that you can download [**here**](https://stackspot.com/).

- Docker: ~20.10.8
- Docker Compose: ~3.8

## **Installation**
To download **template-wordpress-default**, follow the steps below:

**Step 1.** Copy and paste the URL below into your browser/terminal:
```
https://github.com/TheFirstSquad/template-wordpress-default.git
```

## **How to Use**
### Input parameters
The inputs parameters needed to use the template are: 

| **Field**                     | **Value**         | **Description**   |
| :---                          | :---              | :---              |
| Project Name                  | ex.: project-name | Application name  |
| Wordpress Server Port         | ex.: 81           | Web Server port   |
| Wordpress Database Name       | ex.: wp_stackspot | Database Name     |
| Wordpress Database Port       | ex.: 3306         | Database Port     |
| Wordpress Database UserName   | ex.: wp_stackspot | Database User     |
| Wordpress Database Password   | ex.: wp_stackspot | Database Password |
| Wordpress Docker Image        | ex.: 6.0.1        | Docker image name |

 ## Creating the project from the template

 ```bash
stk create app project-name -S stack-wordpress/default
 ```

Wordpress Mapped Folders
>Development related to these components must be carried out in their respective folders

| **Folder Host**   | **Folder in Docker**              | **Description**   |
| :---              | :---                              | :---              |
| ./src/plugins     | /var/www/html/wp-content/plugins  | Plugins folder    |
| ./src/themes     | /var/www/html/wp-content/themes    | Themes folder     |



## Execution of the created project

After creating your project, to build and run the docker containers solution, run the command below in the root of where you find the **docker-compose.yml** file

```bash
docker-compose -f 'docker-compose.yml' up --build
```

Then open http://localhost:81 in your browser.

## References
- [Stackspot documentation](https://docs.stackspot.com/v4.0.0/docs/)
- [Wordpress documentation](https://developer.wordpress.org/)
## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://www.lucasapoena.eti.br/"><img src="https://avatars.githubusercontent.com/u/135553?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Lucas Apoena</b></sub></a><br /><a href="https://github.com/TheFirstSquad/template-wordpress-default/commits?author=lucasapoena" title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!