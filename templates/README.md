# {{ inputs.project_name }}

## **How to Use**
### Input parameters
The inputs parameters needed to use the template are: 

| **Field**                     | **Value**                                 | **Description**   |
| :---                          | :---                                      | :---              |
| Project Name                  | {{ inputs.project_name }}                 | Application name  |
| Wordpress Server Port         | {{ inputs.wordpress_server_port }}        | Web Server port   |
| Wordpress Database Name       | {{ inputs.wordpress_database_name }}      | Database Name     |
| Wordpress Database Port       | {{ inputs.wordpress_database_port}}       | Database Port     |
| Wordpress Database UserName   | {{ inputs.wordpress_database_username }}  | Database User     |
| Wordpress Database Password   | {{ inputs.wordpress_database_password }}  | Database Password |

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

Then open http://localhost:{{ inputs.wordpress_server_port }} in your browser.