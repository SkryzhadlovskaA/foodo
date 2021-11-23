Site can be found as always on: http://clabsql.clamv.jacobs-university.de/~asavu/index.php

Added the updated code, where everything inside of search uses user group9read_only.
To 'suggest', you need to login as admin. Credentials for you to double check are email: admin@foodo.com pass: admin
This form where you enter the credentials is the only input from the website that doesn't require admin login nor does it use read_only user, therefore this would be weak against injection.
To combat this, we used parametized prepared queries as well as checking whether the input contains the character ';'.


