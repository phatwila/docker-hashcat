Fork of https://github.com/dizcza/docker-hashcat

[![Docker Hub](http://dockeri.co/image/b1ker/docker-hashcat)](https://hub.docker.com/r/b1ker/docker-hashcat/)

[Hashcat](https://hashcat.net/hashcat/) git based build (beta/dev) with hashcat utils on Ubuntu 18.04 OpenCL for Nvidia GPUs (`:latest`) and Intel CPU (`:intel-cpu`).

```
docker pull b1ker/docker-hashcat
nvidia-docker run -it b1ker/docker-hashcat /bin/bash

# run hashcat bechmark inside the docker container
hashcat -b
```

## Nvidia GPU

 `docker pull b1ker/docker-hashcat:latest`

## Additional Hashcat utils

Along with the hashcat, the following utility packages are installed:

* [hashcat-utils](https://github.com/hashcat/hashcat-utils) for converting raw Airodump to HCCAPX capture format; info `cap2hccapx -h`
* [hcxtools](https://github.com/zerbea/hcxtools) for inspecting, filtering, and converting capture files;
* [hcxdumptool](https://github.com/ZerBea/hcxdumptool) for capturing packets from wlan devices in any format you might think of; info `hcxdumptool -h`
* [kwprocessor](https://github.com/hashcat/kwprocessor) for creating advanced keyboard-walk password candidates; info `kwp -h`

