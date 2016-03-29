# switchsite

**switchsite** is a bash function for switching between copies of the same or
similar sites hosted in the `/srv/www/` directory.  This allows you to teleport
from deep within the directory structure of one site to the equivalent location
within another site.

## Usage

```bash
switchsite othersite
```

If you are, for example, at `/srv/www/mysite/public_html/somewhere/deep/inside`,
the command above will take you to
`/srv/www/othersite/public_html/somewhere/deep/inside`.

As you might expect, `switchsite mysite` will bring you right back.

## Installation

You will need to put the `switchsite` file somewhere accessible and tell bash
to include it.  Edit your **.bashrc** file and add the following

```bash
. /path/to/switchsite
```

The changes will not take effect until you open a new terminal window.

## Licensing

Copyright 2016 AGH Strategies, LLC

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
