A delicious.com to email gateway
================================

It is intended to be run about hourly. All new links with a specified
tag are mailed to an address.

Configuration
-------------

The first few lines of the del2mail script contain its configuration:

* `USER`: the user whose links are read or all users if left empty
* `TAG`: the tag the links must have
* `MAIL_SERVER`: the name or IP address of the SMTP server
* `RECIPIENTS`: a list of mail recipients
* `SENDER`: a (address, name) 2-tuple of the sender. If the mail goes to a mailing list,
  make sure that the sender is allowed to send to the list.

The script writes to `/var/local`, so make sure that the user
as which the script runs has write permissions there.
