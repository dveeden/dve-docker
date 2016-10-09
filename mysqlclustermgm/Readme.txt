
Run ndb_mgmd:
docker run -d dveeden:ndb74ndbmgmd --name mgm01

Run ndb_mgm:
docker run -it --link suspicious_pasteur:mgm01 dveeden:ndb74ndbmgm

Run ndbmtd:
docker run -d --link boring_euclid:mgm01 dveeden:ndb74ndbmtd
docker run -d --link boring_euclid:mgm01 dveeden:ndb74ndbmtd
