# Examples of using the SDK

The Databricks SDK for Python comes with a number of examples demonstrating how to use the library for various common use-cases, including

* [Using the SDK with OAuth from a webserver](https://github.com/databricks/databricks-sdk-py/blob/main/examples/flask_app_with_oauth.py)
* [Using long-running operations](https://github.com/databricks/databricks-sdk-py/blob/main/examples/starting_job_and_waiting.py)
* [Authenticating a client app using OAuth](https://github.com/databricks/databricks-sdk-py/blob/main/examples/local_browser_oauth.py)

The examples are organized by the Databricks API that they use. Hand-written examples are present in the `examples/` directory.
Generated examples are available in subdirectories, with two main directories corresponding to Account 
and Workspace clients. Inside these main directories, there are subdirectories corresponding to each 
Databricks service.

We welcome contributions of new examples or corrections to existing ones. Before contributing, be aware of the following caveats:
* Examples in service-specific subdirectories are autogenerated. Do not edit these directly; changes will be overwritten the next time SDK code is generated.
* Examples are not automatically tested as part of the CI pipeline. If you add a new example, please test it manually before submitting a PR.
