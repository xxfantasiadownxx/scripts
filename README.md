This collection of scripts is intended to update and maintain Mac OS systems on a network.
<br>
<br>
Directory information:
<br>
<b>update_os</b> - This is the original script to prune user accounts which have been dormant beyond 30 days and update Mac OS to the latest stable release. After the update process, the machine will restart. This script is also used in <i>parallel_updates</i> and <i>update_all</i>.
<br>
<b>update_p-fv</b> - This script is the same as <i>update_os</i> but adds a function to disable notifications to enable FileVault.
<br>
<b>update_all</b> - This is a script that sequentially processes updates via <i>ipaddresses.txt</i> and applies the <i>update_os</i> script to each one.
<br>
<b>parallel_updates</b> - This is a script that processes 5 parallel updates at once via <i>ipaddresses.txt</i> and applies the <i>update_os</i> script to each one.
<br>
<b>credentials.json</b> - This file holds your credentials for the SSH session used in <i>parallel_updates</i> and <i>update_all</i>. You will need to supply your own credentials before use.
<br>
<b>ipaddresses.txt</b> - This file holds the target IP addresses for <i>parallel_updates</i> and <i>update_all</i>. You will need to supply your own IPs before use.
<br>
<b>prune_users</b> - This script simply prunes user accounts which have been dormant beyond 30 days. It is also used within <i>update_os</i>.
