# Activiti BPM demo for Hydra Order Management System (homs)

This repository keeps Activiti BPM demo processes which could be executed with [Hydra Order Management System](https://github.com/latera/homs) (homs).

Requirements:
* [homs](https://github.com/latera/homs)
* [Activiti](http://activiti.org) 5.19.x
* [Latera Activiti extension](https://github.com/latera/activiti-ext)

## Installation

1. Download source code by git:

    ```bash
    git clone https://github.com/latera/homs-demo-processes.git
    ```

2. Zip each project in separate archive:

    ```bash
    ls -d */ | xargs -I{} sh -c 'd=${1%/}; zip -j $d.zip $d/*.bpmn $d/*.yml' -- {}
    ```

3. Deploy each project archive via Activiti admin interface: _Manage_ -> _Deployments_ -> _Upload new_

## License

Copyright (c) 2016 Latera LLC under the [Apache License](https://github.com/latera/activiti-homs-demo/blob/master/LICENSE).
