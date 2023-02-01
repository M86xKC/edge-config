# Microsoft Edge Enterprise Policies for Linux

This repository contains the configuration for Microsoft Edge Enterprise policies on Linux operating system. With these policies, you can control various settings in the browser, such as search, disabling features, privacy, and security settings.

## Setting up Enterprise policies

To set up the policies, you will need to follow these steps:

1. Clone this repository or download the `policies.json` file from this repository.
2. Copy the `policies.json` file to the path `/etc/opt/edge/policies/managed/` on your Linux machine.
3. Modify the configuration file to match your needs.
4. The policies will be automatically applied to Microsoft Edge.
5. To verify that the policies have been applied, navigate to the `edge://policy/` page in the browser.

## Policy Configuration

For reference yoiu can review [Microsoft Edge Browser Policy Documentation](https://learn.microsoft.com/en-us/deployedge/microsoft-edge-policies)

It is important to note that the default configuration is strict and disables several features including:

- Microsoft account & sync
- Sidebar hub & search
- Recommendations & ads
- Shopping coupons & rewards
- Collection & workspaces
- Text prediction & speech recognition
- JavaScript JIT
- Third-party cookies
- Built-in password manager and auto-fill functionality

You can also add `--enable-features=msDiagnosticDataForceOff` to `$XDG_CONFIG_HOME/microsoft-edge-stable-flags.conf` to further restrict the data sent to Microsoft.

## Contributing

This configuration is currently only for Linux operating systems. Contributions are welcome to support MacOS and Windows as well. If you would like to contribute, please submit a pull request with your changes.

## License

This repository is licensed under the GPL-3 License.
