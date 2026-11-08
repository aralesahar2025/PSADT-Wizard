# PSADT Wizard

> **Disclaimer:** PSADT Wizard is an independent community project designed to simplify common PSAppDeployToolkit customization tasks. This project is not affiliated with or endorsed by the PSAppDeployToolkit project. Always validate and test generated deployment configurations before production use.

## Overview

PSADT Wizard is an interactive PowerShell utility that helps administrators accelerate application packaging using PSAppDeployToolkit (PSADT).

Rather than manually editing deployment scripts and configuration variables, the wizard guides administrators through a series of simple questions and automatically applies the selected values to the deployment package.

The goal is to reduce complexity, improve consistency, and help both new and experienced packaging engineers create high-quality deployment packages more efficiently.

---

## Why This Project Exists

PSAppDeployToolkit is one of the most popular Windows application deployment frameworks available today.

While extremely powerful, many administrators spend considerable time manually editing the same deployment information for every package:

- Application name
- Vendor
- Version
- Detection logic
- Package metadata
- Uninstall information
- Installation parameters

PSADT Wizard automates these repetitive tasks and promotes a more consistent packaging experience.

---

## Features

✅ Interactive PowerShell-based wizard

✅ Guided package customization process

✅ Automatic modification of deployment configuration

✅ Faster PSADT package preparation

✅ Consistent deployment standards

✅ Simplified onboarding for new administrators

✅ Support for version-aware deployment logic

✅ Packaging workflow optimization


Packages created using PSAppDeployToolkit can be used with Omnissa Workspace ONE UEM

## Recommended Detection Strategy

Whenever possible, use:

### File Exists + File Version

Benefits:

- Reliable version validation
- Improved upgrade handling
- Reduced false positives
- Better support for unmanaged application scenarios

Using file existence together with version validation can help avoid situations where an older, unmanaged application installation causes deployment detection to incorrectly report success before installation begins.

---

## Requirements

### Operating System

- Windows 10
- Windows 11

### PowerShell

- PowerShell 7.x recommended

### Dependencies

- PSAppDeployToolkit

Download PSAppDeployToolkit from the official project:

https://github.com/PSAppDeployToolkit/PSAppDeployToolkit

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/aralesahar/PSADT-Wizard.git
```

### Change to the Project Directory

```bash
cd PSADT-Wizard
```

### Run the Wizard

```powershell
.\PSADT-Wizard.ps1
```

---

## Usage

1. Download or create a PSADT package.
2. Launch PSADT Wizard.
3. Answer the configuration prompts.
4. Review the generated changes.
5. Validate the package.
6. Test deployment.
7. Deploy using Omnissa Workspace ONE UEM.

---

## Example Workflow

### Package Creation

```text
Application Name: Visual Studio Code
Vendor: Microsoft
Version: 1.144.1
Architecture: x64
```

### Wizard Output

```text
✅ Application information updated
✅ Deployment variables configured
✅ PSADT configuration customized
✅ Package ready for testing
```

---

## Screenshots

### Wizard Startup

![Wizard Startup](screenshots/start.png)

### Package Configuration

![Configuration](screenshots/configuration.png)

### Generated Output

![Output](screenshots/output.png)

---

## Project Goals

- Reduce packaging effort
- Increase deployment consistency
- Simplify PSADT adoption
- Improve administrator productivity
- Encourage deployment best practices

---

## Contributing

Contributions, improvements, bug reports, and feature suggestions are welcome.

If you discover an issue or have an idea that could improve the project, please open an Issue or submit a Pull Request.

---

## Disclaimer

PSADT Wizard is an independent community project created to assist administrators with common PSAppDeployToolkit customization tasks.

This project is not affiliated with, endorsed by, sponsored by, or maintained by the PSAppDeployToolkit project or its contributors.

PSADT Wizard does not include, redistribute, modify, or replace PSAppDeployToolkit. Users must obtain PSAppDeployToolkit separately from the official project source and comply with all applicable licensing terms.

The script performs automated configuration updates based on user input and should be considered an administrative aid rather than a replacement for validation and testing.

Users are responsible for:

- Reviewing generated output
- Validating deployment behavior
- Testing packages before production use
- Ensuring compliance with organizational standards

The author provides this project "as is" without warranty of any kind and assumes no responsibility for any damages, service interruptions, deployment failures, or other consequences resulting from use of this software.

Always test packages thoroughly in a non-production environment before deployment to production systems.

All product names, trademarks, and logos referenced in this project remain the property of their respective owners.

---

## License

This project is licensed under the MIT License.

See the LICENSE file for full details.

---

## Author

**Arale Sahar**

Solutions Consultant

GitHub: https://github.com/aralesahar

---

## Acknowledgments

Special ity for creating and maintaining one of the most widely used Windows application deployment frameworks available today.

This project exists because of the excellent foundation PSAppDeployToolkit provides to the endpoint management community.