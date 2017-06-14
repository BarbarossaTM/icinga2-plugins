```
$ ./check_conntrack_size -h
usage: check_conntrack_size [-h] [--warn WARN] [--crit CRIT]
                            [--no-conntrack {ok,warn,crit,unkn}]

check netfilter conntrack table size

optional arguments:
  -h, --help            show this help message and exit
  --warn WARN, -w WARN  Warning conntrack table usage (percent)
  --crit CRIT, -c CRIT  Critical conntrack table usage (percent)
  --no-conntrack {ok,warn,crit,unkn}
                        Return code when no conntrack is loaded.
```
