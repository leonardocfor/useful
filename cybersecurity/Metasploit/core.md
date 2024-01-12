# Metasploit learning

Main command

```bash
msfconsole
```

#### Modules

Loading modules

```bash
use <module_name>
```

Setting arguments when inside loaded module

See Modules options

```bash
show options
```

See Modules advanced options

```bash
advanced # or show advanced
```

Set options

```bash
set <OPTION> <VALUE>
```

Unset options

```bash
unset <OPTION>
```

Set global options

If a module has the option, then the global value will be applied. Global options might be deleted when logging out msfconsole

```bash
setg <OPTION> <VALUE>
```

Run the module 

```bash
run
```

Run the module in the background

```bash
run -j # explot -j might work too
```

#### Jobs

See runing jobs 

```bash
jobs
```

Kill job 

```bash
job -k <JOB_ID>
```

Kill all jobs

```bash
jobs -K
```



