## Golang Jira Client 

Jira client can operate tasks from specific filter.

### Roadmap:

* profiles
* list task
* watch on new task
* get description
* assing to other person
* add/remove labels
* change due

### Profile context:


```json
[
    {
        "name": "<name_of_profile">,
        "default": true,
        "filter": "fileter",
        "data": {
            "url": "https://localhost:8389",
            "username": "user",
            "password": "password",
        }
    },
    {
        "name": "<name_of_profile">,
        "default": false,
        "data": {
            "url": "https://localhost:8387",
            "username": "user",
            "password": "password",
        },
    },
    .....
]
```

### Cli option tree:

```sh

Global options:
  -p, --profile 

list        show list of task
watch       watch on new task append
get         get details of task
assignee    assignee the task to person
labels      work with labels
due         work with duedates
```


#### list

```sh
> list --help
List Options:
  -f, --follow  Refresh list periodicly. 
  -t, --time    Time to refresh. In seconds.
  -h, --help    Show usecase of list command

```

#### watch
```sh
> watch --help

Watch Options:
  -h, --help    Show usecase of watch command

```

#### get
```sh
> get --help

Get Options:
  -h, --help    Show usecase of get command

```

#### assignee
```sh
> assignee --help

Assignee Options:
  -h, --help    Show usecase of assignee command

```

#### labels
```sh
> labels --help

Labels Options:
  -h, --help    Show usecase of labels command

```

#### due
```sh
> due --help

Due Options:
  -h, --help    Show usecase of due command

```
