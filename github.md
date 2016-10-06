API Error codes
Generic

    200 - OK
    400 - Bad request (invalid input)
    401 - Unauthorized (login required, account locked, permission error)
    403 - Forbidden ( server locked and other reasons )
    419 - This function can only be executed with an CL-account
    405 - Not Allowed (managed server)
    500 - Internal Server Error

6XX - server

    601 - server/details, could not get server details
    602 - server/status, uptime not supported for xen server
    603 - server/create, no payment card
    604 - server/create, not allowed to create more server.
    605 - server/create, failed to create server
    606 - server/delete, failed to delete server
    607 - server/edit, hostname not unique
    608 - server/edit, apply changes failed
    609 - server.php/private/checkTemplateLimits, unknown template
    610 - server, invalid configuration option for current template
    612 - server/clone, cloning not supported on this platform.
    613 - server/clone, failed to create clone
    614 - server/limits, not supported on this platform
    615 - server/resetlimit, not supported on this platform
    616 - server/resetpassword, only supported on OpenVZ
    617 - server/edit, not enough free memory on hypervisor to allow upgrade
    618 - server/edit + server/create, limitation because of api test account
    619 - server/* HnConnectionException
    620 - server/console, server not started
    621 - server , could not find server on serverplatform
    622 - server/create, Could not create server. Maintenance.
    623 - server/backup, Invalid backup type and server platform combination.
    624 - server/create, Password is required for the specified template

7XX - ip

    701 - ip/details,
    702 - ip/take, unable to assign ip to account
    703 - ip/release, unable to release ip from account
    704 - ip/add, ip not on account
    705 - ip/add, ip already assigned to server
    706 - ip/add, ip is not on the same platform as this server
    707 - ip/add, ip is not in the same datacenter as this server
    708 - ip/add, Failed to add ip to server! Contact support@glesys.se
    709 - ip/add, Unable to add ip to stopped vz-server.
    710 - ip/remove, Unable to remove ip from stopped vz-server.
    711 - ip/remove, Unable to remove ip from server (most likely not on a server)
    712 - ip/listfree, Unsupported combination of ipversion/datacenter/platform.
    713 - ip/add, max number of ips per server reached.
    714 - ip/release, Unable to release ip that is locked to account.

8XX - archive

    801 - archive/list, could not list all archives for this account.
    802 - archive/details, could not find this user on this account.
    803 - archive/create, could not create archive
    804 - archive/delete, could not delete archive
    805 - archive/changepassword, could not change password for archive user
    806 - archive/resize, could not resize volume

9XX - domain

    901 - domain/updaterecord, unable to locate zone.
    902 - domain, could not find registrarinfo for domain
    903 - domain, unsupported tld
    904 - domain/register, not allowed to register more domains
    905 - domain/delete, not allowed to delete domain invoiced by glesys that is not expired
    906 - unable to renew domain
    907 - unable to register domain
    908 - unable to transfer domain
    910 - unable to change nameservers
    911 - invalid record type for domain
    912 - not allowed to add arpa domain
    913 - cannot delete domains with active email accounts to email aliases.

10XX - email

    1001 - email/list - unable to account or alias matching filter
    1002 - email/createalias - error when creating alias
    1003 - email/createaccount - error when creating account
    1004 - email/editalias - error when editing alias
    1005 - email/quota - could not get quota for account
    1006 - email/editaccount + email/createaccount - error setting quota
    1007 - email/globalquota - error setting global quota

11XX - livechat

    1101 - unable to post livechat message
    1102 - unable to validate livechat session
    1103 - unable to get livechat messages
    1104 - unable to close livechat session
    1105 - unable to create new session
    1106 - livechat is currently closed
    1107 - this session is no longer active
    1108 - unable to get sessioninfo

12XX - invoice / paymentcard

    1201 - snailmail is only available to sweden, norway, finland and denmark
    1202 - Unable to contact the database of this country to validate vat number.
    1203 - Unable to validate VAT number against European Commissions database.
    1204 - You are not allowed to change the billing period of this account.
    1205 - Invalid invoice number
    1206 - Invalid payment card
    1207 - Card payment error
    1208 - Invoice already payed.
    1209 - Other ongoing payments on this account is preventing this payment from taking place. Please try again later.
    1210 - Invoice validation error
    1211 - Paypal error

13XX - glera

    1301 - unable to find user
    1302 - glera/createuser - user already exists
    1303 - glera/createvhost - vhost already exists
    1304 - unable to find vhost
    1305 - cannot find this ip on this server
    1306 - glera/createuser - invalid masteruser
    1307 - invalid directory

14XX - transaction

    1401 - invalid transaction

15XX - vpn

    1501 - could not create user
    1502 - could not delete user
    1503 - could not change password for user
    1504 - could not find user on account

16XX - user

    1601 - login failed
    1602 - login failed (unknown error)
    1603 - Google Authenticator OTP required
    1604 - Yubikey OTP required
    1605 - Not logged in as a user

17XX - invite

    1701 - Invalid invite code

18XX - Test account

    1801 - Test account already exist

19XX - Network

    1901 - Network in use. Can not delete.

    Contact GitHub API Training Shop Blog About 


