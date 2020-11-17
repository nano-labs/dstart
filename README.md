# dstart - Docker start
Command to select services to start with docker-compose

![Usage gif](https://github.com/nano-labs/dstart/blob/main/imgs/dstart.gif)

## Install
```
pip3 install dstart
```

## Usage
```shell
> dstart
```
- SPACEBAR to select services
- ENTER to start selected services

```shell
$ dstart --help
usage: dstart [-h] [-f FILE] [--print-only] [--extra ...]

Command to select services to start with docker-compose.

optional arguments:
  -h, --help            show this help message and exit
  -f FILE, --file FILE  Specify an alternate compose file (default: docker-compose.yml)
  --print-only          Just print docker-compose command and exit
  --extra ...           Extra arguments will be passed to `docker-compose up` command
```

## How does it work
It uses `docker-compose` command to list all running container then `docker-compose up <SERVICES>` to start them

### See also
[dkill](https://github.com/nano-labs/dkill) - Docker Kill