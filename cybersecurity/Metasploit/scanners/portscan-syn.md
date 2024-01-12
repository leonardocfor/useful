# SYN portscan

Load module

```bash
use auxiliary/scanner/portscan/syn
workspace <WORKSPACE> # Set the workspace
```

Setting options

```bash
set RHOSTS <CIDR>
# hosts -R # If there're hosts in the database
set PORTS 21,22,139,445,443,80
# set PORTS 21-445 # Intervals can be set as well
set THREADS <X>
# Advance options below
set VERBOSE true # See output
set GATEWAY_PROBE_HOST <GATEWAY>
```


