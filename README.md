# PortProxy

A .NET 6 networking project containing TCP and UDP proxy implementations, a desktop application and a Windows service host.

## Architecture

| Path | Responsibility |
| --- | --- |
| `PortProxy/` | Proxy implementations, configuration models and shared services |
| `PortProxy.App/` | Desktop application |
| `PortProxy.WinService/` | Windows service and gRPC server startup |

The core project references gRPC client tooling and SQL Server connectivity packages.

## Build from source

Open `PortProxy.sln` in Visual Studio on Windows with the .NET 6 SDK and relevant desktop development tooling. Restore packages and build the solution. Consult the [original documentation](Port%20Proxy.docx) for further context.

## Status and security

Existing implementation on a legacy .NET target. Build and runtime behavior have not been independently verified. Test using authorized endpoints and review authentication, listener binding and firewall rules before deployment.
