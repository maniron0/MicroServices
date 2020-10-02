# MicroServices Nuances

- Service Registry
  - Service Register
  - Service Unregister
  - Service Health Monitoring
- Service Discovery
  - HTTP based (HTTP API for location and port information)
  - DNS based [PTR (service types to named service instances), SRV (location and port), TXT (additional metadata) records]
  
- Service Registry Approaches
  - Self registry (Client is responsible for registering/de-registering itself with SR) 
  - Using Sidecar (A sidecar process monitors the main process and updates it state in SR accordingly)
  - 3rd party Service (A 3rd party service monitors a service or a set of services and updates their state in SR accordingly)
- Service Discovery Approaches
  - Client Side Discovery (Client -> SR)
  - Server Side Discovery (Client -> LB -> SR)
