## Custom Runtimes

Custom Runtime can be used to _extend_ Kyma Serverless Functions to run unsupported language. Custom Runtimes allows users to provide their own prebuilt function images and skip the normal function build process. Essentially allowing users to run their own images as Kyma Serverless workloads.


#### Perquisites

Currently, the custom runtime need to implement the following to be able to run successfully as a Serverless Function workload:
- Expose the workload endpoint on `http:8080`.
- Provide liveness and readiness check endpoints at `/healthz`.


### Runtimes:
- [Golang Hello World](https://github.com/moelsayed/gohello)