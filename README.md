# Nextron YAML IOC Specification

This repository contains the official specification for the IOC (Indicator of Compromise) YAML format used in Nextron products such as THOR.

## What is this?

The YAML IOC format is a standardized way to define threat intelligence indicators in a structured, human-readable format. This specification enables security analysts and threat hunters to create portable IOC rules that can detect various types of malicious artifacts including:

- **File indicators**: File paths, names, and patterns.
- **Network indicators**: C2 domains, IPs.
- **System indicators**: Mutexes, named pipes, events.
- **Hash indicators**: File hashes (MD5, SHA1, SHA256, Imphash).

## Benefits for Users

- **Future Proof**: Consistent format across different Nextron tools and environments, starting with THOR.
- **Portability**: IOC rules can be shared and reused across different deployments.
- **Validation**: JSON schema ensures rule correctness and prevents common errors.
- **Flexibility**: Support for various IOC types with customizable scoring and filtering.
- **Documentation**: Built-in fields for references, descriptions, and metadata.

## Main Files

- **[yaml-ioc-schema.json](yaml-ioc-schema.json)**: The main JSON Schema file that defines the complete IOC YAML specification.
- **testdata/**: Example IOC rules demonstrating valid and invalid formats for testing purposes.

## Documentation

For detailed information on using IOC rules with THOR, see the [THOR Manual](https://thor-manual.nextron-systems.com/en/v11/signatures/ioc-types.html).