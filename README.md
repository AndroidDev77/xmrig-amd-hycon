# HYCminer AMD

HYCminer is a high performance Hycon (HYC) OpenCL miner, forked from [XMRig](https://github.com/xmrig/xmrig) release v2.6.1.
Mining algorithm has been changed to Lyra2.

* This is the **AMD GPU** mining version, 

#### Table of contents
* [Features](#features)
* [Download](#download)
* [Usage](#usage)
* [Algorithm variations](#algorithm-variations)
* [Build](https://github.com/team-hycon/xmrig-amd/wiki/Build)
* [Common Issues](#common-issues)
* [Other information](#other-information)
* [Contacts](#contacts)

## Features
* Currently running Lyra2 Hash
* High performance.
* Support for backup (failover) mining server.
* Automatic GPU configuration.
* GPU health monitoring (clocks, power, temperature, fan speed) 
* Nicehash support.
* It's open source software.

## Download
* Binary releases: TBA
* Git tree:https://github.com/AndroidDev77/xmrig-amd-hycon/xmrig-amd.git
    * Clone with `https://github.com/AndroidDev77/xmrig-amd-hycon/xmrig-amd.git` :hammer: [Build instructions](https://github.com/team-hycon/xmrig-amd/wiki/Build).

## Usage
See the example `config.json` to configure the miner.

### Command line options
```
  -a, --algo=ALGO           cryptonight (default) or cryptonight-lite
  -o, --url=URL             URL of mining server
  -O, --userpass=U:P        username:password pair for mining server
  -u, --user=USERNAME       username for mining server
  -p, --pass=PASSWORD       password for mining server
  -k, --keepalive           send keepalived for prevent timeout (need pool support)
  -r, --retries=N           number of times to retry before switch to backup server (default: 5)
  -R, --retry-pause=N       time to pause between retries (default: 5)
      --opencl-devices=N    list of OpenCL devices to use.
      --opencl-launch=IxW   list of launch config, intensity and worksize
      --opencl-affinity=N   affine GPU threads to a CPU
      --opencl-platform=N   OpenCL platform index
      --no-color            disable colored output
      --donate-level=N      donate level, default 5% (5 minutes in 100 minutes)
      --user-agent          set custom user-agent string for pool
  -B, --background          run the miner in the background
  -c, --config=FILE         load a JSON-format configuration file
  -l, --log-file=FILE       log all output to a file
      --nicehash            enable nicehash support
      --print-time=N        print hashrate report every N seconds
      --api-port=N          port for the miner API
      --api-access-token=T  access token for API
      --api-worker-id=ID    custom worker-id for API
  -h, --help                display this help and exit
  -V, --version             output version information and exit
```

Also you can use configuration via config file, default **config.json**. You can load multiple config files and combine it with command line options.

## Other information
* No HTTP support, only stratum protocol support.
* No TLS support.
* Default donation 5% (5 minutes in 100 minutes) can be reduced to 1% via command line option `--donate-level`.

## Contacts
* curquhart90@gmail.com
* hycon@glosfer.com
* [site](https://www.hycon.io)
* [reddit](https://www.reddit.com/r/HYCON)
* [facebook](https://www.facebook.com/teamHycon)
* [instagram](https://www.instagram.com/teamhycon)
* [medium](https://www.medium.com/@teamhycon)
* [twitter](https://www.twitter.com/teamhycon)
