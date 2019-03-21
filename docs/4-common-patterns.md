# Common container patterns

### [Back](../README.md)

| Pattern diagram | Description |
| ----------------| ------------ |
| <img src="./images/sidecar.png" width="420"> | Sidecar pattern extends and enhance the main container. |
| <img src="./images/adapter.png" width="420"> | Adapter present the outside world with a simplified, homogenized view of an application. |
| <img src="./images/ambassador.png" width="420"> | Ambassador containers proxy communication to and from a main container. |
| <img src="./images/leader-elect.png" width="420"> | A set of leader-election containers, each one co-scheduled with an instance of the application that requires leader election, can perform election amongst themselves, and they can present a simplified HTTP API over localhost to each application container that requires leader election
 |
| <img src="./images/scatter-gather.png" width="420"> | This root fans the request out to a large number of servers to perform computations in parallel. Each shard / server returns partial data, and the root gathers this data into a single response to the original request.
 |
| <img src="./images/work-queue.png" width="420"> | The work queue pattern dictates that you split up a big task into smaller tasks to reduce running time. The code that does the processing work can be packed into a worker container, and then you can spin up several pods at the same time.
 |