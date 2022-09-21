## wait-for-py

Wait on a TCP connection with no system dependencies other than Python 3.
This is super tiny, so just vendor it.

## Example usages

```sh
wait-for some-server:1000 other-server:2000
WAIT_FOR=localhost:8080,localhost:8081 ./docker/wait-for -n 2
```

## Description

```
usage: wait-for [-h] [-d DELAY] [-n NUM_TRIES] [targets ...]

Wait for stuff to boot with no system dependencies other than Python 3. Example usages: wait-for server:3000 WAIT_FOR=localhost:8080,localhost:8081 wait-for -n 2

positional arguments:
  targets               The targets to poll, e.g. "localhost:8081"

options:
  -h, --help            show this help message and exit
  -d DELAY, --delay DELAY
                        Number of seconds to delay between attempts
  -n NUM_TRIES, --num-tries NUM_TRIES
                        Number of times to try each target
```
