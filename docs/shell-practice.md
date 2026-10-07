# Supporting shell practice

A separate archive contained 30 screenshots of terminal exercises, without a
written report. They show permissions, umask, text filters, archives, network
inspection, hostnames, and service/firewall inspection. Some screenshots contain
an instructor-derived working-directory name, so they are not republished.

## Skills demonstrated

| Topic | Evidence in the original exercises |
|---|---|
| Files and directories | mkdir, touch, tree, cp, mv |
| Permissions | chmod, ls -l, umask, chown and groups |
| Text processing | grep character classes and anchors, cut, head, tail and wc |
| Archives | tar creation, listing and extraction, including correction of failed attempts |
| System inspection | ip, nmcli, hostname, hostnamectl and systemctl |
| Firewall inspection | firewall-cmd service listing |

## Useful corrections

- `grep '[0-9]' file.txt` finds lines containing a digit. Anchors such as `^`
  and `$` refer to the start and end of a line; place them inside a quoted pattern.
- `grep 'me$' file.txt` searches for lines ending in `me`. Putting `$` before
  the pattern is not the same operation.
- `cut -d: -f2 file.txt` selects the second colon-delimited field; a field or
  character selection is needed for `cut` to do useful work.
- The original `hostnamectl show hostname` attempt failed. The evidence then
  shows `hostnamectl hostname` displaying the hostname.
- `systemctl status ssh` failed in this Fedora exercise. The completed networking
  lab uses the service name `sshd`.

These notes describe the submitted exercises and their visible corrections.
They are not a claim that new shell commands were executed during preparation.
