# presto-cli [![][layers-badge]][layers-link] [![][version-badge]][dockerhub-link]

[layers-badge]: https://images.microbadger.com/badges/image/teradatalabs/presto-cli.svg
[layers-link]: https://microbadger.com/images/teradatalabs/presto-cli
[version-badge]: https://images.microbadger.com/badges/version/teradatalabs/presto-cli.svg
[dockerhub-link]: https://hub.docker.com/r/teradatalabs/presto-cli

## Overview

This image contains CLI for defined version of Presto.

## Examples

To use examples below please set following environment variables:
`PRESTO_VERSION=    # version of Presto CLI to be used, usually same as Presto Server version that can be found in Presto WebUI`
`PRESTO_HOST=        # host on which Presto Master is visible`
`PRESTO_PORT=        # port on which Presto Master is visible (most likely 8080)`

Run:
`docker run -i -t teradatalabs/presto-cli:$PRESTO_VERSION --server $PRESTO_HOST:$PRESTO_PORT`

Run single query:
`docker run -i -t teradatalabs/presto-cli:$PRESTO_VERSION --server $PRESTO_HOST:$PRESTO_PORT --execute "$QUERY"`

Build:
`docker build -t teradatalabs/presto-cli --build-arg PRESTO_VERSION=0.165-t .`

## Oracle license

By using this image, you accept the Oracle Binary Code License Agreement for Java SE available here:
[http://www.oracle.com/technetwork/java/javase/terms/license/index.html](http://www.oracle.com/technetwork/java/javase/terms/license/index.html)


