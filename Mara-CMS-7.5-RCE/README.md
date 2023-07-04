# Mara CMS 7.5 - Authenticated

This is a script that automates the exploitation of Mara CMS, version 7.5. 

The arguments required to run the script include:

```
-u -> the URL of the Mara CMS instance
-li -> the local IP address of your listening host
-lp -> the local port that your host is listening on
-c -> your session cookie
	* A session cookie is required, but it can be easily obtained by logging into /cms?login=admin with the default credentials of admin:changeme
```

The script will upload the shell to the `/cms/blog/shell.php` URI.

Before running the script, ensure your listener has been started. 

## References

* https://www.exploit-db.com/exploits/48780
* Tiny PHP reverse shell stolen from: https://gist.github.com/rshipp/eee36684db07d234c1cc
