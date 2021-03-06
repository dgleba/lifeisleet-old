# Life Is Leet

[![Build Status](http://img.shields.io/travis/lifeisleet/lifeisleet.svg?style=flat)](https://travis-ci.org/lifeisleet/lifeisleet)
[![Dependency Status](http://img.shields.io/gemnasium/lifeisleet/lifeisleet.svg?style=flat)](https://gemnasium.com/lifeisleet/lifeisleet)
[![Code Climate](https://codeclimate.com/github/lifeisleet/lifeisleet/badges/gpa.svg)](https://codeclimate.com/github/lifeisleet/lifeisleet)
[![Test Coverage](https://codeclimate.com/github/lifeisleet/lifeisleet/badges/coverage.svg)](https://codeclimate.com/github/lifeisleet/lifeisleet)
[![Issues](https://img.shields.io/github/issues/lifeisleet/lifeisleet.svg?style=flat)](https://github.com/lifeisleet/lifeisleet/issues)

CMS for podcasters.

## Development

### Requirements

 * [Docker](https://www.docker.com/)
 * [Docker Compose](https://docs.docker.com/compose/)

On OS X:

 * [DLite](https://github.com/nlf/dlite)
 * Installing Docker and Docker Compose through [Homebrew](http://brew.sh/) is
   recommended.

### Setup

```bash
$ git clone https://github.com/lifeisleet/lifeisleet.git && cd $_
$ bin/setup
$ docker-compose up
```

The web server will be listening on port 3000 of your Docker host.

### Testing

```bash
$ docker-compose run --rm -e RAILS_ENV=test web bin/rake db:setup
$ docker-compose run --rm web bin/rspec
```

## Copyright

Copyright (C) 2015 Life Is Leet.

This program is free software: you can redistribute it and/or modify it under
the terms of the GNU Affero General Public License as published by the Free
Software Foundation, either version 3 of the License, or (at your option) any
later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE. See the GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License along
with this program. If not, see
[http://www.gnu.org/licenses/](http://www.gnu.org/licenses/).
