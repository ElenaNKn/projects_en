# API specification for managing access to secret data (JSON-RPC format)

## Project description

The project contains complete specification for the method, which provide the ability to add, receive and delete data. It takes into account different levels of access of users. For example, only superAdmin can delete data. Specification also provide a versioning mechanism for the method.

**Method accepts the following parameters:**
- action: action type (add, get, delete)
- dataID: data identifier
- userData: data to add (optional)
- accessLevel: access level of a user (user, admin, superAdmin)
- language: language, in which messages and notifications are to be output ("EN", "RU", "DE", "FR", "ES")

The specification specifies parameters, results and errors messages for the method. It also contains sample requests and responses for each use case. It is written in **json-rpc 2.0 format**.

This specification may be used while working on developing an API for secure storage that stores secret user data. 

A tool to investigate the specification: https://playground.open-rpc.org/