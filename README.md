# Bulk Mailer

Command line tool for sending email using a data file and email template as inputs. It's email-merge for admins.


## Author

Geof Gowan, geof@jgbg.org, April 4, 2007

## Usage

    USAGE: bulk-mail -data ... -from ... -template ... <optional flags>

    REQUIRED:
        -data     The text file with email addresses and other variables
                 to be merged with the email template.
        -from     The email address to put in the From: line
        -template The email template file.

    OPTIONAL:
        -smtp     Alternate smtp server. The default is smtp.ufl.edu
        -max      Maximum messages per SMTP session. Default is 30.
        -wait     Set pause in seconds between SMTP sessions. Default is 1.
        -local    If delivering to local users, this will disable the
                 check for \@ in recipient addresses.
        -quiet    Suppress progress feedback and errors.
        -stealth  If set, will pause 1 second between each sent email.
        -verbose  Provide feedback for successfully sent email.

For more details run `perldoc bulk-mail`
