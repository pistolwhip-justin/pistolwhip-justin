# HIDPP 2.0

pixl edited this page on Jun 9, 2020 · [1 revision](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0/_history)

# Features

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#features)

## 0x0000: Root

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#0x0000-root)

_This feature ID on the device will always be 0._

### Function 0: Get Feature

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-0-get-feature)

**Arguments:** Byte 0: Feature ID MSB; Byte 1: Feature ID LSB

**Returns:** Byte 0: Feature Index; Byte 1: Flags (OHE-----) where O is obsolete, H is hidden, and E is engineering; Byte 2: Feature version

### Function 1: Get Protocol Version

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-1-get-protocol-version)

**Arguments:** Byte 0 & 1: Zero for padding; Byte 2: Ping data (to be returned)

**Returns:** Byte 0: Protocol Version (Major); Byte 1: Target SW; Byte 2: Ping data

**Target SW:** Bit 7: SW defined by feature 0x0030; Bit 3-6 are unused; Bit 2: Preference Manager; Bit 1: Gaming Software; Bit 0: Device Manager

### Event 0: No operation

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#event-0-no-operation)

Sent to prevent device from entering low power mode.

## 0x0001: Feature set

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#0x0001-feature-set)

### Function 0: Get number of features

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-0-get-number-of-features)

**Returns:** Byte 0: Number of features

### Function 1: Get feature

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-1-get-feature)

**Arguments:** Byte 0: Feature index

**Returns:** Byte 0: Feature ID MSB; Byte 1: Feature ID LSB

## 0x0002: Feature info

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#0x0002-feature-info)

#### Function 0: Get base feature?

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-0-get-base-feature)

If the feature ID is a newer version of another feature, it should return the feature ID of its base version.

**Arguments:** Byte 0: Feature ID MSB; Byte 1: Feature ID LSB

**Returns:** Byte 0: Base Feature ID MSB; Byte 1: Base Feature ID LSB

## 0x0003: Device FW version

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#0x0003-device-fw-version)

### Function 0: Get number of firmwares

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-0-get-number-of-firmwares)

**Returns:** Byte 0: Number of firmwares; Byte 1-4: Unit UUID; Byte 5: Protocol Support MSB (reserved); Byte 6: Protocol Support (Lower nibble bits are: USB, Unifying, BTLE, Bluetooth)

### Function 1: Get firmware version

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-1-get-firmware-version)

**Arguments:** Byte 0: Firmware index

**Returns:** Byte 0: Firmware type; Byte 1-3: ASCII Firmware Prefix; Byte 4: Firmware Number; Byte 5: Revision; Byte 6-7: Build Number; Byte 8: Active entity; Byte 9-10: PID; Byte 11-15: Extra versioning info

Firmware types: 0 = Main; 1 = Bootloader; 2 = Hardware

## 0x0005: Device name

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#0x0005-device-name)

### Function 0: Get length

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-0-get-length)

**Returns:** Byte 0: Length of device name

### Function 1: Get device name

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-1-get-device-name)

**Arguments:** Byte 0: Character index

**Returns:** 16 bytes of the device name as a null-terminated string starting from the given index

## 0x0020: Reset

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#0x0020-reset)

#### Function 0: Nothing?

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-0-nothing)

#### Function 1: Reset to default settings

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-1-reset-to-default-settings)

## 0x0021: Crypto identifier

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#0x0021-crypto-identifier)

#### Function 0: Returns part 1 of crypto identifier?

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-0-returns-part-1-of-crypto-identifier)

#### Function 1: Returns part 2 of crypto identifier?

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-1-returns-part-2-of-crypto-identifier)

#### Function 2: Generates new crypto identifier?

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-2-generates-new-crypto-identifier)

## 0x1000: Battery status

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#0x1000-battery-status)

### Function 0: Get battery percentage?

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-0-get-battery-percentage)

**Returns:** Byte 0: Battery percentage, Byte 1: ???, Byte 2: Charging flag

### Function 1: ???

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-1-)

**Returns:** Byte 0-4: ???

#### Sample Device Outputs

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#sample-device-outputs)

MX Master (50%): 04 04 c0 28 0a

T400 (80%): 04 00 c0 b4 0a

## 0x1814: Change host

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#0x1814-change-host)

### Function 0: Get host information

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-0-get-host-information)

**Returns:** Byte 0: Number of supported hosts, Byte 1: Current host (zero-indexed)

### Function 1: Set host

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-1-set-host)

**Arguments:** Byte 0: Host to switch to (zero-indexed)

**Returns:** Connection terminates.

## 0x1b00: Reprogram controls

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#0x1b00-reprogram-controls)

### Function 0: Get number of buttons

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-0-get-number-of-buttons)

**Returns:** Byte 0: Number of buttons

### Function 1: Get button info

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-1-get-button-info)

**Arguments:** Byte 0: Button index

**Returns:** Byte 0: Control ID MSB; Byte 1: Control ID LSB; Byte 2: Task ID MSB; Byte 3: Task ID LSB; Byte 4: Flags; Byte 5: Position (if F key, else 0); Byte 6: Group; Byte 7: Group remap mask (bit no. corresponds to group no.); Byte 8: Can be reprogrammed as Gesture button

**Flags:** Bit 7: virtual; Bit 6: persistent divert; Bit 5: temporary divert; Bit 4: Reprogrammable; Bit 3: Affected by Fn Toggling; Bit 2: Hotkey; Bit 1: Function key; Bit 0: Mouse button

### Function 2: ???

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-2-)

**Arguments:** Byte 0: ???

**Returns:** Byte 0: Argument Byte 0

### Function 3: ???

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-3-)

**Arguments:** Byte 0: ???

**Returns:** Byte 0: Argument Byte 0

## 0x1b03: Reprogram controls v3

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#0x1b03-reprogram-controls-v3)

Refer to 0x1b00 for functions

### Event 0: Diverted button state change

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#event-0-diverted-button-state-change)

**Returns:** Array of 0-4 16-bit CIDs?

## 0x1b04: Reprogram controls v4

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#0x1b04-reprogram-controls-v4)

### Function 0: Get number of buttons

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-0-get-number-of-buttons-1)

Same as 0x1b00 function 0

### Function 1: Get button info

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-1-get-button-info-1)

Same as 0x1b00 function 1

### Function 2: Get CID reporting info

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-2-get-cid-reporting-info)

**Arguments:** Byte 0: CID MSB; Byte 1: CID LSB

**Returns:** Byte 0: CID MSB; Byte 1: CID LSB; Byte 2: Divert Flags [---R-P-T] (R is raw XY, P is persistent, T is temporary); Byte 3: Remap CID MSB; Byte 4: Remap CID LSB

### Function 3: Set CID reporting

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#function-3-set-cid-reporting)

**Arguments:** Byte 0: CID MSB; Byte 1: CID LSB; Byte 2: Divert Flags [---URUPUT] (U updates the flag to the right if set, R is raw XY, P is persistent, T is temporary); Byte 3: Remap CID MSB; Byte 4: Remap CID LSB

**Returns:** Echoes parameters

### Event 0: Diverted button state change

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#event-0-diverted-button-state-change-1)

**Returns:** Array of 0-4 16-bit CIDs

### Event 1: Diverted Raw XY state change

[](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0#event-1-diverted-raw-xy-state-change)

**Returns:** Byte 0: dx MSB; Byte 1: dx LSB; Byte 2: dy MSB; Byte 3: dy LSB

###