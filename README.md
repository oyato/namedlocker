# namedlocker

Package namedlocker implements in-memory named locks. See https://oya.to/namedlocker for docs.

# Install

    go get oya.to/namedlocker

# Usage

    package test


    func Example() {
        sto := Store{}
        sto.Lock("my-key")
        defer sto.Unlock("my-key")

        // do some work...
    }
