# Transferencing files

#!/bin/bash

function print_usage {
    echo -e "USAGE: aws-igenomes.sh\n" \
        "\t\t[-g <genome name>]\n" \
        "\t\t[-s <source name>]\n" \
        "\t\t[-b <build name>]\n" \
        "\t\t[-t <reference type>]\n" \
        "\t\t[-o <output directory>]\n" \
        "\t\t[-d (dry run, no downloads)]\n" \
        "\t\t[-q (quiet mode, non-interactive)]\n" \
        "\t\t[-h (usage help)]\n\n" \
        "All command line flags are optional. If not specified\n" \
        "and not running in quiet-mode, the script will prompt\n"\
        "for input and show available options.\n\n" \
        "Please note that this script requires the AWS command\n" \
        "line tools to be installed and configured for authenticated\n" \
        "access.\n" >&2
}
