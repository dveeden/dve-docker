
Run ndb_mgmd:
docker.io run -d dveeden:ndb72ndbmgmd --name mgm01

Run ndb_mgm:
docker.io run -it --link suspicious_pasteur:mgm01 dveeden:ndb72ndbmgm

Run ndbmtd:
docker.io run -d --link boring_euclid:mgm01 dveeden:ndb72ndbmtd
docker.io run -d --link boring_euclid:mgm01 dveeden:ndb72ndbmtd
