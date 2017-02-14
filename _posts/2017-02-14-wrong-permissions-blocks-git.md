Wrong permissions for authorized_keys block git access via public key over ssh
==============================================================================

During playing around with a hosted Git environment I run into an issue that the access to the remote requested the password for the git user.

	git@12.34.56.78's password:
	Permission denied (publickey,password).
	fatal: Could not read from remote repository.

The reason was accidentally changed permissions (666) of the key ```file ~/.ssh/authorized_keys```.

	-rw-rw-rw- 1 git git  393 Feb 12 21:41 authorized_keys

After setting it back to 600 

	chmod 600 authorized_keys
	ls -la
	-rw------- 1 git git  393 Feb 12 21:41 authorized_keys

the remote didn't request any password and used the authentication via public key.




