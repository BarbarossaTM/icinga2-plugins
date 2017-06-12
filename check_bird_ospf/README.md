$ ./check_bird_ospf -h
usage: check_bird_ospf [-h] [--proto {4,6}] [--protocol PROTOCOL]
                       [--interfaces_down_ok LIST]
                       [--interfaces_down_ok_file FILENAME]
                       [--ignore_missing_file]

check bird OSPF sessions

optional arguments:
  -h, --help            show this help message and exit
  --proto {4,6}, -p {4,6}
                        IP protocol version to check
  --protocol PROTOCOL, -P PROTOCOL
                        Bird OSPF protocol instance name to check
  --interfaces_down_ok LIST
                        List of interfaces which are OK to have no OSPF
                        neighbor. Provide a space separated list.
  --interfaces_down_ok_file FILENAME
                        List of interfaces which are OK to have no OSPF
                        neighbor. Provide one interfaces per line.
  --ignore_missing_file
                        Ignore a possible non-existent file given as
                        --interfaces_down_ok_file
