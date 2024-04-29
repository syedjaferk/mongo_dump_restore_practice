### To Practice mongodump and mongorestore.

docker compose -f mongo.yml up
./mgodatagen -f full-bson.json
mongodump --uri="mongodb://localhost:27017"


For Mongodump:
docker exec <mongodb container> sh -c 'mongodump --archive' > db.dump

docker exec e8758216e1a1 sh -c 'mongodump --archive' > db.dump
docker exec 55a0ed465d7d sh -c 'mongodump --archive' > db.dump
55a0ed465d7d



For Restore:

docker exec -i <mongodb container> sh -c 'mongorestore --archive' < db.dump
docker exec -i 82614b8a0046 sh -c 'mongorestore --archive' < db.dump_version_4.2.3

