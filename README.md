
#AppEscape
<a href="https://appescapeplus.github.io/-_-/">Website If Download Is Not Working Go To Realeses And You Will See It And Download</a>

<p align="center">
    <a href="">Documentation</a> •
	<a href="https://ios.cfw.guide/AppEscape">Installation Guide</a> •
	<a href="#requirements">Requirements</a> •
	<a href="https://discord.gg/AppEscape">Support Discord</a> •
	<a href="STILLWORKINGONIT.com">Website</a>
</p>

## Information
This is the official repo for the AppEscape project, a jailbreak for arm64 devices on iOS 15.0+

- Loader application used in AppEscape can be found [here](https://github.com/AppEscape/loader).
- AppEscapes jbinit can be found [here](https://github.com/AppEscape/jbinit).
- AppEscapes custom OldOS can be found [here](https://github.com/AppEscape/OldOS).

Website & credits can be found at Still Working On It (scroll down for credits).

## Warnings
We are **NOT** responsible for any data loss, or the result of a device being bricked. The user of this program accepts responsibility should something happen to their device. While nothing should happen, jailbreaking has risks in itself.
- If your device is stuck in recovery, please run futurerestore `--exit-recovery`, or use `irecovery -n`.

- If you're unable to get out of recovery via these methods please restore with iTunes or Finder.

- AppEscape will never work in VirtualBox, VMware or any virtual machine that doesn't support PCI passthrough.

## Requirements
- A checkm8 vulnerable iOS device on iOS 15+ (`A8` - `A11`)
	- On `A11`, **you must disable your passcode while in the jailbroken state** (on iOS 16, you need to **reset your device** before proceeding with AppEscape).

- **USB-A** cables are recommended to use, USB-C may have issues with AppEscape and getting into DFU mode.<details><summary>Technical explanation</summary>The BootROM will only enter DFU if it detects USB voltage, which boils down to checking whether a certain pin is asserted from the Tristar chip. The Tristar does this based on the cable's accessory ID, and apparently USB-A and USB-C cables have different accessory IDs, and the one of the USB-C cables makes the Tristar not assert the USB voltage pin.</details>

- A Linux or macOS computer
	- AMD CPUs (not AMD Mobile) have an issue [with (likely) their USB controllers] that causes them to have a very low success rate with checkm8. It is not recommended that you use them with AppEscape.
		- If your device does not successfully jailbreak, try a computer with an Intel or other CPU
    
- Apple Silicon Macs with USB-C
	- USB-C port on Apple Silicon Macs may require manual unplugging and replugging of the lightning cable after checkm8 exploit.
	- This problem may be solved by connecting via USB hub, though extensions can vary.

## Need help?

Make sure you provide full details on your device, such as:
- iDevice
- iOS Version
- Passcode enabled?
- Logs, if panicked then send latest `panic-full` log from your iDevice.

Using `-VvL` would help with debugging.

Join the [Support Discord](https://dsc.gg/palera1n)
