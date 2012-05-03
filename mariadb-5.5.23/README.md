# MariaDB Spec file

mariadb.5.5.23.spec is the upstream oracle spec file modified to work with mariadb 5.5.23. I have sent this to mariadb, and hopefully they will modify it some more (descriptions and whatnot) and distribute in the next version of maria.


# Testing Twitter patches

!! I do not recomend anyone use this spec file for anything other than testing. !!

mariadb.5.5.23-twitter.spec uses twitter's numactl patch, which sets the numa interleave up properly, as well as twitter's innodb_buffer_pool_populate patch which allocates the entire buffer pool at once rather than incrementally. I'm pretty sure both these patches will be making their way into MariaDB very soon if not already. BUT I want to test them now so here we are. More information here:

http://blog.jcole.us/2012/04/16/a-brief-update-on-numa-and-mysql/

!! I do not recomend anyone use this spec file for anything other than testing. !!

