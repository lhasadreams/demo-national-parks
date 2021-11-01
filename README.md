## Running in docker studio

[![HIPAA](https://app.soluble.cloud/api/v1/public/badges/0a49695f-2b75-4944-be9d-0ab14f70a126.svg)](https://app.soluble.cloud/repos/details/github.com/lhasadreams/demo-national-parks)  [![IaC](https://app.soluble.cloud/api/v1/public/badges/9246a5f5-404a-4a9b-ba71-5704bdf4c3db.svg)](https://app.soluble.cloud/repos/details/github.com/lhasadreams/demo-national-parks)  [![CIS](https://app.soluble.cloud/api/v1/public/badges/4889f312-4227-4cf4-8f61-e8acfc7125d8.svg)](https://app.soluble.cloud/repos/details/github.com/lhasadreams/demo-national-parks)  

```
# Windows
$env:HAB_DOCKER_OPTS="-p 8080:8080"
# Linux
export HAB_DOCKER_OPTS="-p 8080:8080"


hab studio enter
start_parks

```

Open your browser to `https://localhost:8080/national-parks` to see the app.

## Starting the supervisor in studio
```
hab sup run > /hab/sup/default/sup.log &
```

## Pre-Demo checklist

* Have studio open
* build at least once
* start np-mongodb
* Have open SSH sessions to hab1-3 and docker host
* increment NP version and commit (but do not push)
* make sure mongodb container is running on docker host
* have browser tabs open to my origins, local app, and azure app
