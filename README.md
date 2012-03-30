# errdb-rb

A Ruby client library for the [Errdb](http://github.com/erylee/errdb).

## Getting started

You can connect to Errdb by instantiating the `Redis` class:

    require "errdb"

    errdb = Errdb.new({:host => "localhost", :port => 7272})

Once connected, you can start running commands against Errdb:

    errdb.insert "key", 9999, {"metric1" => 10, "metric2" => 20}

    errdb.fetch "key", "metric1,metric2", 0, 999999999


