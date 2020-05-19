
To download file from remote server using SFTP. Creates a maximum of 16 connections.

	aria2c -x 16 -s 40 --ftp-user=<SSH USERNAME> --ftp-passwd=<SSH PASSWORD> "sftp://<HOST>:<PORT>/my/file.tar.gz"

