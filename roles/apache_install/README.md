
`tasks/main.yml` - the main list of tasks that the role executes.

`handlers/main.yml` - handlers, which may be used within or outside this role.

`defaults/main.yml` - default variables for the role (see Using Variables for more information). These variables have the lowest priority of any variables available, and can be easily overridden by any other variable, including inventory variables.

`vars/main.yml` - other variables for the role (see Using Variables for more information).

`files/main.yml` - files that the role deploys.

`templates/main.yml` - templates that the role deploys.

`meta/main.yml` - metadata for the role, including role dependencies.