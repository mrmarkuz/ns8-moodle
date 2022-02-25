# ns8-moodle

Start a Moodle instance.

The module uses https://github.com/bitnami/bitnami-docker-moodle

## Install

Instantiate the module with:

    add-module ghcr.io/nethserver/moodle:latest 1

The output of the command will return the instance name.
Output example:

    {"module_id": "moodle1", "image_name": "moodle", "image_url": "ghcr.io/nethserver/moodle:latest"}

## Configure

Let's assume that the moodle instance is named `moodle1`.

Launch `configure-module`, by setting the following parameters:
- `<MODULE_PARAM1_NAME>`: <MODULE_PARAM1_DESCRIPTION>
- `<MODULE_PARAM2_NAME>`: <MODULE_PARAM2_DESCRIPTION>
- ...

Example:

    api-cli run module/moodle1/configure-module --data '{}'

The above command will:
- start and configure the moodle instance
- (describe configuration process)
- ...

Send a test HTTP request to the moodle backend service:

    curl http://127.0.0.1/moodle/

## Uninstall

To uninstall the instance:

    remove-module --no-preserve moodle1

## Testing

Test the module using the `test-module.sh` script:


    ./test-module.sh <NODE_ADDR> ghcr.io/nethserver/moodle:latest

The tests are made using [Robot Framework](https://robotframework.org/)
