# Plummet

This project aims to look at interop between Roughtime clients and servers,
providing the means to run both against each other.

## Development and Running

All implementations are provided as git submodules, you'll need to clone this
repository using the `--recurse-submodules`, or if you have already cloned it,
you'll need to run `git submodule update --init --recursive`.

You'll need Docker as well as [Poetry](https://python-poetry.org) installed.
To get started, clone this repository, then run:
```bash
poetry shell
poetry install
```

You can then run `poetry run plummet -h` to see the help information.

To build all the implementations:
```bash
docker compose -f implementations/docker-compose.yml build
```
This will take a while, and a lot of disk space.

## Licence

Copyright 2024-

Licensed under the Apache License, Version 2.0 (the "License"); you may not use
this file except in compliance with the License.  You may obtain a copy of the
License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed
under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
CONDITIONS OF ANY KIND, either express or implied.  See the License for the
specific language governing permissions and limitations under the License.
