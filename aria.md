
To download file from remote server using SFTP. Creates a maximum of 16 connections.

	aria2c -x 16 --ftp-user=<SSH USERNAME> --ftp-passwd=<SSH PASSWORD> "sftp://<HOST>:<PORT>/my/file.tar.gz"
	

If there are multiple servers serving same file, you can use `-s` flag. Refer aria2c [manpage](https://aria2.github.io/manual/en/html/aria2c.html#options)

