https://digitalprivacy.diy/
====== rsync ======

[[https://rsync.samba.org/|rsync]] is an [[https://www.opensource.org/|open source]] utility that provides fast incremental file transfer. rsync is freely available under the [[https://rsync.samba.org/GPL.html|GNU General Public License]]. 


===== Package =====

<code>
pacman -S rsync
</code>


===== SSH =====


<code>
rsync --recursive --links --times --owner --group --itemize-changes --partial --progress --human-readable --verbose --stats /local/path user@host:~/path/
</code>

**From ssh to local**:
<code>
rsync --recursive --links --times --owner --group --itemize-changes --partial --progress --human-readable --verbose --stats user@host:~/path/ /local/path
</code>

**Short**:
<code>
rsync -rltogiPhv --stats /local/path user@host:~/path/
</code>
<code>
rsync -rltogiPhv --stats user@host:~/path/ /local/path
</code>

**Different port**:
<code>
rsync -rltogiPhv --stats -e "ssh -p PORTNUMBER" /local/path user@host:~/path/
</code>

See what each option does - https://man.archlinux.org/man/rsync.1#OPTION_SUMMARY


===== Daemon =====

==== Credentials ====

<code>
echo "$user:$password" > /etc/rsyncd.secrets
chmod 400 /etc/rsyncd.secrets
</code>

==== Config ====

Change ''$user''.

<code>
nano /etc/rsyncd.conf
</code>
<code>
[archive]
path = /path/
comment = Archive
timeout = 300
read only = false
# http user if you want to have access via web
#uid = 33
#gid = 33
# Run a script before and after a connection
#pre-xfer exec = /root/before_script.sh
#post-xfer exec = /root/after_script.sh
# Security
auth users = $user      
secrets file = /etc/rsyncd.secrets
# Optional
#hosts allow = 192.168.1.0/255.255.255.0
</code>

==== Start ====

<code>
systemctl enable --now rsyncd.service
</code>


==== Command ====

Change ''$DAEMONUSER'' and ''$DAEMONHOST''.

<code>
rsync --rltogiPhv --stats /local/path rsync://$DAEMONUSER@$DAEMONHOST/archive/path/
</code>


===== Backup =====

Go to our [[en:backup:server#rsync|backup]] tutorial.

https://digitalprivacy.diy/