# Architecture

## Internal Dependencies

- `packet_edit_meme.c` -> `pedit_primitive.h`
- `pedit_primitive.c` -> `pedit_primitive.h`
- `test_cve.c` -> `pedit_primitive.h`

## External Imports

- `packet_edit_meme.c` -> elf.h, errno.h, fcntl.h, sched.h, stdio.h, stdlib.h, string.h, sys/stat.h, sys/wait.h, unistd.h
- `pedit_primitive.c` -> arpa/inet.h, errno.h, fcntl.h, linux/if_ether.h, linux/netlink.h, linux/pkt_cls.h, linux/pkt_sched.h, linux/rtnetlink.h, linux/tc_act/tc_pedit.h, net/if.h, stdio.h, stdlib.h, string.h, sys/sendfile.h, sys/socket.h, sys/stat.h, unistd.h
- `pedit_primitive.h` -> stdint.h, sys/types.h
- `test_cve.c` -> fcntl.h, stdint.h, stdio.h, string.h, unistd.h
