# Reports

# Exploit Title: Joomla! Component GMapFP 3.5* - Unauthenticated Arbitrary File Upload
# Google Dork: inurl:''com_gmapfp''
# Date: 2020-03-27
# Exploit Author: ThelastVvV
# Vendor Homepage:https://gmapfp.org/
# Version:Version J3.5 /J3.5free
# Tested on: ubuntu

# Description:

An attacker can access the upload function of the application without authenticating to the application and also can upload files due the issues of unrestricted file uploads which can be bypassed by changing the content-type and name file too double extensions (file.html.gif)

# PoC:


Version J3.5
http://127.0.0.1/index.php?option=com_gmapfp&controller=editlieux&tmpl=component&task=edit_upload


https://i.imgur.com/TUHu1Oa.jpg


#once the attacker can locate the unauthenticated file upload form then the attacker can bypass the restriction by changing content-type and name file double extensions file.html.gif then can open file.html

# Impact
the attacker can upload malicious files can cause defacement of the site or uploading large amount of file til causes denial of service attack to Webapp/Server

# Dir File Path:
http://127.0.0.1///images/stories/gmapfp/test.html.gif
http://127.0.0.1///images/stories/gmapfp/test.html
http://127.0.0.1///images/gmapfp/test2.html.gif
http://127.0.0.1///images/gmapfp/test2.html.gif


# Issues are fixed,Please update to Last Version

