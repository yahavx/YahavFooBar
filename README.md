![build status](https://travis-ci.org/yahavx/mindreader.svg?branch=master)
![coverage](https://codecov.io/gh/yahavx/mindreader/branch/master/graph/badge.svg)
![docs](https://readthedocs.org/projects/mindreader/badge/?version=latest)

# mindreader

Yahav's final project for Advanced System Design course.

## Table of Contents

* [Prerequities]
* [Installation](#installation)
* [Quickstart](#quickstart)
* [Usage](#usage)
* [Documentation](#documentation)
* [Support](#support)

## Installation

1. Clone the repository and enter it:

    ```sh
    $ git clone git@github.com:yahavx/mindreader.git
    ...
    $ cd mindreader/
    ```

2. Run the installation script and activate the virtual environment:

    ```sh
    $ ./scripts/install.sh
    ...
    $ source .env/bin/activate
    [mindreader] $ # you're good to go!
    ```

3. To check that everything is working as expected, run the tests:

    ```sh
    [mindreader] $ pytest tests/
    ...
    ```

## Quickstart
After finishing the [installation](#installation) step, run the ```run-pipeline``` script:

```sh
[mindreader] $ ./scripts/run-pipeline.sh
...
Everything is ready!
[mindreader] $
```

Now upload some snapshots from the [client](/mindreader/client/README.md):
```sh
[mindreader] $ python -m mindreader.client snapshot.mind.gz
...
All the 1024 snapshots were sent successfully!
[mindreader] $ 
```
After than, visit http://127.0.0.1:8080/ to see the results. You can also use the [CLI](/mindreader/cli/README.md) or 
the [API](/mindreader/api/README.md) to view the data.

## Usage

The project contains one package, `mindreader`, which provides the following sub-packages:
* [`client`](/mindreader/client/README.md) :mega: - sends cognition snapshots to the server.
* [`server`](/mindreader/server/README.md) :calling: - receives cognition snapshots from the client, and handles them.
* [`parsers`](/mindreader/parsers/README.md) :hammer: - processes snapshots received from the server.
* [`saver`](/mindreader/saver/README.md) :key: - saves processed data to the database.
* [`api`](/mindreader/server/README.md) :book: - an API to consume the data.
* [`cli`](/mindreader/cli/README.md) :memo: - a CLI that consumes the API.
* [`gui`](/mindreader/gui/README.md) :computer: - allows to visualize the data comfortably.

Click on your desired package to be forwarded to the matching readme, which supply a simple yet more extensive 
description, and also usage examples of the basic functionality.

For a more detailed explanation, as well as necessary information to manage the code, check the
[official documentation](https://mindreader.readthedocs.io/en/latest/).

## Documentation

The complete documentation for the project can be found [here](https://mindreader.readthedocs.io/en/latest/).

## Support

Reach out to me at one of the following places!
* Email :email: - yahavxx@gmail.com
* Twitter :bird: - @yahavxx