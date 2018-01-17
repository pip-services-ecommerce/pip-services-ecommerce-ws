# <img src="https://github.com/pip-services/pip-services/raw/master/design/Logo.png" alt="Pip.Services Logo" style="max-width:30%"> <br/> Workspace for eCommerce Pip.Services

This is a workspace for [eCommerce Pip.Services](https://github.com/pip-services-ecommerce) 
implemented in 5 different languages: .NET, Java, Node.js, Go and Python.

The workspace enables build, test, and release across the following projects:

- **pip-services-creditcards-node** - Credit cards microservice in Node.js
- **pip-clients-creditcards-node** - Client to Credit cards microservice in Node.js
- **pip-services-invoices-node** - Invoices microservice in Node.js
- **pip-clients-invoices-node** - Client to Invoices microservice in Node.js
- **pip-facade-ecommerce-node** - eCommerce REST facade in Node.js

## Installation

- Install **pip-tasks-ps**, **pip-tasks-common-ps** and **pip-tasks-node-ps** Powershell modules, 
add them to **PSModulePath** and import into Powershell

- Clone this workspace to local disk
```bash
> git clone https://github.com/pip-services-ecommerce/pip-services-ecommerce-ws.git
```

- Got to the workspace folder and clone component repositories
```bash
> piptask clone -workspace
```

## Usage

- Setting default workspace
```bash
> pipuse <Path to this workspace>
```

- Start and stop ecommerce services
```bash
> piptask start -component pip-services-creditcards
> piptask stop -component pip-services-creditcards
```

- Building all components
```bash
> piptask build -all
```

- Test all components
``` bash
> piptask test -all
```

- Check out changes from remote repository
```bash
> piptask pull -all
```

- Check in changes to remote repository
```bash
> piptask push -m <Changes comment> -all
```

## Acknowledgements

The eCommerce Pip.Services are created and maintained by **Sergey Seroukhov**
