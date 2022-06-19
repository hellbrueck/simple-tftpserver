# simple-tftpserver

*Warning: Does not work yet*

We use the docker (alpine tftp server)[https://hub.docker.com/r/pghalliday/tftp] for the implementation.

with option --rm we always create a new image. be aware that we loose all data on the ftp server. use option -d to run detached.

	docker run --rm -p 69:69/udp pghalliday/tftp
	
use option -v /var/tftpboot:/var/tftpboot for persistence
