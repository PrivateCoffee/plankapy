# plankapy

A python 3 based API for controlling a self-hosted Planka instance

This is a fork of the original [plankapy](https://github.com/hwelch-fle/plankapy)
project by [hwelch-fle](https://github.com/hwelch-fle) that primarily focuses on
making the project a pip installable package.

[Original Docs](https://hwelch-fle.github.io/plankapy/plankapy.html)

## Installation

```bash
pip install git+https://git.private.coffee/PrivateCoffee/plankapy.git
```

## Usage

```python
from plankapy import Planka, User

planka = Planka('http://localhost:3000', 'username', 'password')
users = User(planka)

for user in users.get():
    print(user)
```

Refer to the [original docs](https://hwelch-fle.github.io/plankapy/plankapy.html)
for more information.

## Rest API Source

### Routes

https://github.com/plankanban/planka/blob/master/server/config/routes.js

### Models

https://github.com/plankanban/planka/tree/master/server/api/models

### Helpers

https://github.com/plankanban/planka/tree/master/server/api/helpers
