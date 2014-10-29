# Sandbox Runtime

[Sandbox](https://getsandbox.com) is a platform to quickly and easily create or generate web service mocks, with instant deploy, collaborative build, and debugging tools for API developers. [More info - https://getsandbox.com](https://getsandbox.com)

Sandbox Runtime is the core processing component of the Sandbox product, it is responsible for executing HTTP requests against your definition files (main.js etc) and templates (template.liquid) to produce a response. 

This project consists of both the core runtime code, and a lightweight wrapper to simplify command line use. The compiled version is around 10mb and can be run on mac and linux. 

## Installation

The code can be cloned and compiled by itself (Gradle is used for dependency management) or you can just download the compiled and packaged binary which can be run from the command line on a supported OS.

[Latest compiled binary](https://s3-us-west-2.amazonaws.com/getsandbox-assets/runtime-binary.tar)

### Dependencies

* _Java 8 Update 20 or later_ - important! you actually might not have this, it is pretty recent.
* Mac or Linux

### Commands

The CLI currently supports one action `sandbox run` which will start the runtime with the base directory being the current directory.

```
Commands:
run      Starts a sandbox runtime in the current working directory.

Options:
--port=<port number>
--base=<base directory> (Overrides working directory)
--verbose (Increases logging verbosity, full request and response bodies etc)
```

## Getting Started

For a basic example checkout the `examples` directory, more detail is available on the Sandbox [Getting Started](https://getsandbox.com/docs/getting-started) and the [API Definition](https://getsandbox.com/docs/sandbox-api) pages.

## License

MIT