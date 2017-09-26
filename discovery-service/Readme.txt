rancher-compose --url http://192.168.2.34:8888/v2-beta/projects/1a5  --access-key DE6451A54AEFC2A7D0F0 --secret-key fEnzGyqJR23ZAbdAxb7413R4iu3mjATs7VVPnk7W -f docker-compose.yml -p Applications up --upgrade -p -c -d


http://rancher.com/docs/rancher/latest/en/cattle/upgrading/#in-service-upgrade

-f docker-compose.yml
  --file, -f [–file option –file option]	Specify an alternate compose file (default: docker-compose.yml) [$COMPOSE_FILE]
-p Applications
  --project-name, -p	Specify an alternate project name (default: directory name)


up --upgrade -p -c -d

up
  up    Bring all services up

--upgrade
  --upgrade, -u, --recreate	Upgrade if service has changed
-p
  --pull, -p Before doing the upgrade do an image pull on all hosts that have the image already
-c
  --confirm-upgrade, -c	Confirm that the upgrade was success and delete old containers
-d
 -d	Do not block and log
