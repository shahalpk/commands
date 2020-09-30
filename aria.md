
To download file from remote server using SFTP. Creates a maximum of 16 connections. `-s` is for number of parallel connections and `-x` is for number of parallel connections per server. Since in our case we're downloading from same server it should be same.

	aria2c -s 16 -x 16 --ftp-user=<SSH USERNAME> --ftp-passwd=<SSH PASSWORD> "sftp://<HOST>:<PORT>/my/file.tar.gz"
	



