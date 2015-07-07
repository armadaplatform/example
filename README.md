# example

`example` is a very simple service that can be used to test various Armada features.
It is written using Node.js and can serve as an example service for that platform.


# API (REST)

* `/echo/[text]` - Returns [text].
* `/` - Returns list of container's environment variables in json format.


# Building and running the service.

    armada build example
    armada run example


# Using the service.

Using the IP address and port shown by `armada run example` we can run:

    curl 192.168.3.45:49176/echo/foo

We should get `foo` as a result.
