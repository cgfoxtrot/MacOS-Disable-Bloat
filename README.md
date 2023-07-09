# disableBloat.sh

## Description

`disableBloat.sh` is a script designed to disable unwanted services on macOS, optimizing system performance and improving security by reducing the attack surface. It disables various unnecessary GUI settings and user/system services that may consume system resources and pose potential security risks.

## Features

- Disables GUI-related animations and tweaks for improved performance.
- Disables a comprehensive list of user and system services known to be unnecessary for most users.

## Prerequisites

Before using `disableBloat.sh`, you need to disable macOS System Integrity Protection (SIP) as it restricts system modifications. Here are the steps to disable SIP:

1. Restart your macOS device.
2. While your device is restarting, press and hold the **Command (⌘) + R** keys until the Apple logo appears.
3. This will boot your Mac into **Recovery Mode**.
4. From the top menu, select **Utilities > Terminal**.
5. In the Terminal window, type the following command and press **Enter**:

```shell
csrutil disable

Restart your Mac to exit Recovery Mode.

## Usage

To use `disableBloat.sh` and disable unwanted services on macOS, follow these steps:

1. Open the Terminal application on your macOS device. You can find it in the **Applications > Utilities** folder or use the search function in Spotlight (`Command (⌘) + Space`) and type "Terminal".

2. Download the `disableBloat.sh` script by cloning the repository or downloading the script file directly.

3. Navigate to the directory where you downloaded the `disableBloat.sh` script using the `cd` command. For example, if the script is in your Downloads folder, you would use the following command:

```shell
cd ~/Downloads

Make the script executable by running the following command:

```shell
chmod +x disableBloat.sh

Disable macOS SIP by following the instructions mentioned in the "Prerequisites" section.

Run the script using the following command:

```shell
./disableBloat.sh

The script will start disabling the unwanted services and optimizing your macOS system. It may prompt for your administrator password during the process.

Once the script completes, reboot your macOS device for the changes to take effect.

## Reverting Changes

If you wish to revert the changes made by the `disableBloat.sh` script, follow these steps:

1. Open the Terminal application on your macOS device.

2. Navigate to the directory where you downloaded the `disableBloat.sh` script.

3. Run the script with the `--revert` option using the following command:

```shell
./disableBloat.sh --revert

The script will revert the changes made to the disabled services.

Reboot your macOS device for the changes to take effect.

## Security Considerations

By disabling unnecessary services, `disableBloat.sh` helps reduce the attack surface and potentially mitigates security risks on your macOS device. However, please note that modifying system services can have unintended consequences, and it's recommended to have a backup of your important data before running the script.

## Contributions

Contributions are welcome! If you have any improvements or suggestions for the script, feel free to open an issue or submit a pull request.

## License

This script is released under the [MIT License](LICENSE).




