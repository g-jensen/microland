# plan

The idea is to make real projects and then aggregate all of the microservices/tooling here. This way, while making a project, I can keep in mind that it needs to be general enough to put here in microland, but it also forces me to only put microservices here that actually have a use.

## per-service features

* from day one:
  * logs/traces/metrics 
  * docker/kubernetes
* default communication protocol between services is gRPC over HTTP/2
  * multiple transfer medium implementations
    * Normal TCP sockets
    * Unix domain sockets (UDS)
    * Optionally:
      * Named pipes
      * Shared memory
* every service is also a human/LLM-friendly CLI tool
* tests for every service
  * unit/integration
  * component (testing a single service through its interface)
  * E2E (testing multiple services working together through their interface(s))
  * mutation
  * performance
* service discovery

