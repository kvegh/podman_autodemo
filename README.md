# podman_autodemo
Podman automation with Ansible

notes: usecase 1: 

  130  cat ~/right_start 
  131  podman run -d  --rm --name quarkus_test -e POSTGRESQL_USER=quarkus_test -e POSTGRESQL_PASSWORD=quarkus_test -e POSTGRESQL_DATABASE=quarkus_test -p 5432:5432 postgresql-12
  132  podman run -d  --rm --name nodejs_test -e POSTGRESQL_USER=quarkus_test -e POSTGRESQL_PASSWORD=quarkus_test -e POSTGRESQL_DATABASE=quarkus_test -e POSTGRESQL_SERVICE_HOST=192.168.122.31 -p 8080:8080 quay.io/rbaumgar/nodejs-postgresql-persistent 
  133  podman ps 

