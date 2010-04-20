== fail2ban ==

This module allows you to submit IP addresses to the firewall, to stop
them comment spamming your site.


== Requirements ==

To make use of fail2ban you will need to install the fail2ban system utility.
For most distributions it is already packaged. See http://www.fail2ban.org/
for more info.

In the contrib/ directory you will find a configuration snippet to add to
your /etc/fail2ban/jail.conf and a filter to add to /etc/fail2ban/filter.d

These are pre-configured to firewall any matching addresses for 1 week.

The filter is disabled by default in jail.conf.

The system utility and this module are pre-configured with localhost
whitelisted. The module also automatically whitelists the IP address of the
administrator who enabled it on the site.


== Installation ==

Extract the module to sites/*/modules and enable it via the module admin
page.


== Configuration ==

Browse to http://localhost/?q=admin/settings/fail2ban to change
fail2ban settings.

You will see a new checkbox appear on the comments administration page.


== Authors ==

Peter Lieverdink <me@cafuego.net>


== License ==

http://www.gnu.org/licenses/gpl-2.0.html


