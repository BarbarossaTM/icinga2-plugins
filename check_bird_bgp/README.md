```
$ ./check_bird_bgp -h
usage: check_bird_bgp [-h] [--proto {4,6}] --asn ASN [--ibgp] [--ibgp_w RANGE]
                      [--ibgp_c RANGE] [--ebgp] [--ebgp_w RANGE]
                      [--ebgp_c RANGE] [--disabled_ok]
                      [--sessions_down_ok LIST]
                      [--sessions_down_ok_file FILENAME]
                      [--ignore_missing_file]

check bird iBGP sessions

optional arguments:
  -h, --help            show this help message and exit
  --proto {4,6}, -p {4,6}
                        IP protocol version to check
  --asn ASN, -A ASN     Local AS number
  --ibgp, -i            Check iBGP sessions
  --ibgp_w RANGE        Warning interval for down iBGP sessions
  --ibgp_c RANGE        Critical interval for down iBGP sessions
  --ebgp, -e            Check eBGP sessions
  --ebgp_w RANGE        Warning interval for down eBGP sessions
  --ebgp_c RANGE        Critical interval for down eBGP sessions
  --disabled_ok         Treat sessions disabled in bird as OK.
  --sessions_down_ok LIST
                        List of sessions which are OK to be down. Provide a
                        space separated list.
  --sessions_down_ok_file FILENAME
                        List of sessions which are OK to be down. Provide one
                        interfaces per line.
  --ignore_missing_file
                        Ignore a possible non-existent file given as
                        --interfaces_down_ok_file
```
