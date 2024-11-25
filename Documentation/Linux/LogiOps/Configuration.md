# Configuration

pixl edited this page on Jan 13, 2022 · [12 revisions](https://github.com/PixlOne/logiops/wiki/Configuration/_history)

Logid uses a standard libconfig-style config file stored in `/etc/logid.cfg` by default (although you launch logid with the -c option to change it).

The config style may change in the future, however backwards-compatibility will be maintained.

For a sample config, see [logid.example.cfg](https://github.com/PixlOne/logiops/blob/master/logid.example.cfg).

`:` and `=` are used for defining variables and are interchangeable. (e.g. `name: "foo";` is the same as `name = "foo";`)

# Ignoring Devices

[](https://github.com/PixlOne/logiops/wiki/Configuration#ignoring-devices)

Devices can be ignored from being detected and used in logid. To ignore a device, create a field called `ignore` as an array of the PIDs of the devices you want to ignore.

e.g. `ignore: [0x00a7]`

# Defining Devices

[](https://github.com/PixlOne/logiops/wiki/Configuration#defining-devices)

Devices are defined in an array field called `devices`. This array consists of objects that define a device.

e.g. `devices: ( { device object }, { device object } ... );`

## Device Object

[](https://github.com/PixlOne/logiops/wiki/Configuration#device-object)

The following are a list of fields that a device object contains.

### name

[](https://github.com/PixlOne/logiops/wiki/Configuration#name)

This is a required string field that defines the name of the device. To get the name of the device, launch logid with the device connected and it should print out a message with the device name. (e.g. `name: "MX Master";`)

### buttons

[](https://github.com/PixlOne/logiops/wiki/Configuration#buttons)

This is an optional array field that defines the mappings for buttons.

e.g. `buttons: ( { button object }, { button object } ... );`

#### Button Objects

[](https://github.com/PixlOne/logiops/wiki/Configuration#button-objects)

##### cid

[](https://github.com/PixlOne/logiops/wiki/Configuration#cid)

This is a required integer field that defines the Control ID of the button that is being remapped. (e.g. `cid: 0xc4;`)

##### action

[](https://github.com/PixlOne/logiops/wiki/Configuration#action)

This is a required object field that defines the new action of the button. (e.g. `action: { ... };` )

Refer to the actions section for more information.

### dpi

[](https://github.com/PixlOne/logiops/wiki/Configuration#dpi)

This is an optional integer/array field that defines the DPI for a mouse that supports adjustable DPI. (e.g. `dpi: 1000;`)

If your mouse has multiple sensors, you may define separate DPIs for those sensors by using an array and placing the value in the sensor's index (e.g. sensor 0: 1000 dpi, sensor 1: 800 dpi -> `dpi: [1000, 800]`)

### smartshift

[](https://github.com/PixlOne/logiops/wiki/Configuration#smartshift)

This is an optional object field that defines the SmartShift settings for a mouse that supports it.

```
smartshift:
{
    on: true;
    threshold: 30;
    default_threshold: 30;
};
```

#### on

[](https://github.com/PixlOne/logiops/wiki/Configuration#on)

This is an optional boolean field that defines whether SmartShift should be activated. (`true` for SmartShift, `false` for free-spin).

#### threshold

[](https://github.com/PixlOne/logiops/wiki/Configuration#threshold)

This is an optional integer field between 1-255 that defines the threshold required to change the SmartShift wheel to free-spin.

#### default_threshold

[](https://github.com/PixlOne/logiops/wiki/Configuration#default_threshold)

This is an optional integer field between 1-255 that defines the mouse's default threshold required to change the SmartShift wheel to free-spin.

### hiresscroll

[](https://github.com/PixlOne/logiops/wiki/Configuration#hiresscroll)

This is an optional object field that defines the HiRes mouse-scrolling settings for a device that supports it.

```
hiresscroll:
{
    hires: true;
    invert: false;
    target: false;
};
```

#### hires

[](https://github.com/PixlOne/logiops/wiki/Configuration#hires)

This is an optional boolean field that defines whether the mouse wheel should be high resolution or not.

#### invert

[](https://github.com/PixlOne/logiops/wiki/Configuration#invert)

This is an optional boolean field that defines whether to invert the mouse wheel.

#### target

[](https://github.com/PixlOne/logiops/wiki/Configuration#target)

This is an optional boolean field that defines whether mousewheel events should send as an HID++ notification or work normally (`true` for HID++ notification, `false` for normal usage). This option must be set to true to remap the scroll wheel action.

#### up

[](https://github.com/PixlOne/logiops/wiki/Configuration#up)

This is a gesture that defines the action that will be taken when the scroll wheel is moved up (down if inverted). Refer to the Actions/Gestures section for further info. To function, this field requires target to be enabled.

### down

[](https://github.com/PixlOne/logiops/wiki/Configuration#down)

This is a gesture that defines the action that will be taken when the scroll wheel is moved down (up if inverted). Refer to the Actions/Gestures section for further info. To function, this field requires target to be enabled.

### thumbwheel

[](https://github.com/PixlOne/logiops/wiki/Configuration#thumbwheel)

This is an optional object field that defines the thumb wheel settings on a device that supports it (e.g. MX Master 3).

Some devices will not support the proxy, touch, and tap fields. Thumb wheel capabilities can be determined by running logid in debug mode and looking at the output.

#### divert

[](https://github.com/PixlOne/logiops/wiki/Configuration#divert)

This is a boolean field that determines whether the thumb wheel should be handled by logid (`true`) or the OS (`false`).

#### invert

[](https://github.com/PixlOne/logiops/wiki/Configuration#invert-1)

This is a boolean field that determines whether the thumb wheel's scrolling should be diverted.

#### left

[](https://github.com/PixlOne/logiops/wiki/Configuration#left)

This is an optional gesture that defines the action that will be taken when the scroll wheel is moved left (right if inverted). Refer to the Actions/Gestures section for further info. To function, this field requires divert to be enabled.

#### right

[](https://github.com/PixlOne/logiops/wiki/Configuration#right)

This is an optional gesture that defines the action that will be taken when the scroll wheel is moved right (left if inverted). Refer to the Actions/Gestures section for further info. To function, this field requires divert to be enabled.

#### proxy

[](https://github.com/PixlOne/logiops/wiki/Configuration#proxy)

This is an optional action that defines what will occur when the user is in proximity of the thumb wheel. (will be pressed upon entering proximity, released upon leaving). Refer to the Actions section for further info.

#### touch

[](https://github.com/PixlOne/logiops/wiki/Configuration#touch)

This is an optional action that defines what will occur when the user touches the thumb wheel. (will be pressed upon touching the thumb wheel, released upon letting go). Refer to the Actions section for further info.

#### tap

[](https://github.com/PixlOne/logiops/wiki/Configuration#tap)

This is an optional action that defines what will occur when the user taps the thumb wheel once. (Pressed and immediately released after tap). Refer to the Actions section for further info.

# Actions

[](https://github.com/PixlOne/logiops/wiki/Configuration#actions)

### type

[](https://github.com/PixlOne/logiops/wiki/Configuration#type)

This is a required string field that defines the type of action. (e.g. `type: "None";`). The following is a list of possible actions with their additional fields.

## None

[](https://github.com/PixlOne/logiops/wiki/Configuration#none)

This does nothing. There are no additional fields.

## Keypress

[](https://github.com/PixlOne/logiops/wiki/Configuration#keypress)

This maps press and release events of a button to a list of keys/buttons.

### keys

[](https://github.com/PixlOne/logiops/wiki/Configuration#keys)

This is a required string/integer array/list field that defines the keys to be pressed/released. For a list of key/button strings, refer to [linux/input-event-codes.h](https://github.com/torvalds/linux/blob/master/include/uapi/linux/input-event-codes.h). (e.g. `keys: ["KEY_A", "KEY_B"];`). Alternatively, you may use integer keycodes to define the keys.

Please note that these event codes work in a US (QWERTY) keyboard layout. If you have a locale set that does not use this keyboard layout, please map it to whatever key it would be on a QWERTY keyboard. (e.g. "KEY_Z" on a QWERTZ layout should be "KEY_Y")

## Gestures

[](https://github.com/PixlOne/logiops/wiki/Configuration#gestures)

This action disables mouse movement while the button is pressed and allows you to assign actions for each direction. The possible directions are `Up`, `Down`, `Left`, `Right`, and `None`.

Note that any button can be used as a gesture button if the device supports gestures.

Additionally, some scroll wheels can have their up/down or left/right scrolls mapped to some gestures. Gesture modes will state their scroll wheel compatibility in the documentation.

### gestures

[](https://github.com/PixlOne/logiops/wiki/Configuration#gestures-1)

This is a required array of gesture objects that map a direction to a gesture mode and an action.

e.g. `gestures: ( { gesture object }, { gesture object } ... );`

#### direction

[](https://github.com/PixlOne/logiops/wiki/Configuration#direction)

This is a required string field in a gesture object that defines the direction of the gesture. (e.g. `direction: "Up"`)

#### threshold

[](https://github.com/PixlOne/logiops/wiki/Configuration#threshold-1)

This is an optional integer field that determines the number of pixels at which a gesture should activate. (e.g. `threshold: 50`). This value must be greater than 0. If not set or set to an invalid value, the threshold will default to 50 pixels.

#### mode

[](https://github.com/PixlOne/logiops/wiki/Configuration#mode)

This is an optional string field that defines the mode of the gesture. This field defaults to `OnRelease` if it is omitted.

The following is a list of gesture modes:

##### NoPress

[](https://github.com/PixlOne/logiops/wiki/Configuration#nopress)

This mode does nothing. The `action` field is ignored when this mode is used. This gesture is compatible with scroll wheels.

##### OnRelease

[](https://github.com/PixlOne/logiops/wiki/Configuration#onrelease)

This mode presses and releases an action when the gesture button is released. This gesture is not compatible with scroll wheels.

##### OnInterval

[](https://github.com/PixlOne/logiops/wiki/Configuration#oninterval)

This mode presses and releases an action after the mouse is moved every n pixels (where n is the integer field `interval`). This gesture is compatible with scroll wheels.

##### OnThreshold

[](https://github.com/PixlOne/logiops/wiki/Configuration#onthreshold)

Activates once the `threshold` is met, and never again.

##### Axis

[](https://github.com/PixlOne/logiops/wiki/Configuration#axis)

This mode maps a gesture movement to an axis. The axis is defined as a string (e.g. "REL_WHEEL") in the `axis` field and the multiplier for its movement is defined in the `axis_multiplier` field. For a list of axis strings, refer to [linux/input-event-codes.h](https://github.com/torvalds/linux/blob/master/include/uapi/linux/input-event-codes.h). This gesture is compatible with scroll wheels.

#### action

[](https://github.com/PixlOne/logiops/wiki/Configuration#action-1)

This is a mandatory field that defines the action the gesture uses. This can be any action other than `Gestures`. Refer to the entire Actions section for more details.

## ToggleSmartShift

[](https://github.com/PixlOne/logiops/wiki/Configuration#togglesmartshift)

This action toggles the SmartShift scrolling feature when pressed. There are no additional fields.

## ToggleHiresScroll

[](https://github.com/PixlOne/logiops/wiki/Configuration#togglehiresscroll)

This action toggles high resolution scrolling when pressed. There are no additional fields.

## CycleDPI

[](https://github.com/PixlOne/logiops/wiki/Configuration#cycledpi)

This action cycles between the given DPIs.

### dpis

[](https://github.com/PixlOne/logiops/wiki/Configuration#dpis)

This is a mandatory integer array field that defines what DPIs to cycle through. (e.g. `dpis: [800, 1000, 1200];`)

### sensor

[](https://github.com/PixlOne/logiops/wiki/Configuration#sensor)

This is an optional field that will determine what sensor the DPI will switch on. This value defaults to 0. In almost all cases, this does not need to be used.

## ChangeDPI

[](https://github.com/PixlOne/logiops/wiki/Configuration#changedpi)

This action increments the DPI by the value given in the `inc`.

### inc

[](https://github.com/PixlOne/logiops/wiki/Configuration#inc)

This is an integer array field that defines what to increase the DPI by.

### sensor

[](https://github.com/PixlOne/logiops/wiki/Configuration#sensor-1)

See the CycleDPI `sensor` field.

## ChangeHost

[](https://github.com/PixlOne/logiops/wiki/Configuration#changehost)

This action changes the host to a specified host if the device supports changing hosts.

### host

[](https://github.com/PixlOne/logiops/wiki/Configuration#host)

This field may either be an integer representing the host number (one-indexed, as shown on the bottom of the mouse), "next" to go to the next host number, or "prev"/"previous" to go to the previous host number. (e.g. `host = 2;` or `host = "next";`).

# Miscellaneous

[](https://github.com/PixlOne/logiops/wiki/Configuration#miscellaneous)

### workers

[](https://github.com/PixlOne/logiops/wiki/Configuration#workers)

This is an optional field that determines the number of worker threads that logid's workqueue uses. (e.g. `workers = 4;`)

This defaults to 4 if no value is given.

**Warning:** Decreasing the worker thread count is likely to result in reduced performance and counter-intuitively, more threads being created (since the workqueue will run a task in a new thread if it is busy for more than 500ms).

### io_timeout

[](https://github.com/PixlOne/logiops/wiki/Configuration#io_timeout)

This is an optional field that determines how how many milliseconds device I/O will wait for before timing out. (e.g. `timeout = 2000;`)

This defaults to 2000 ms if left blank.

### Pages 5

- [Home](https://github.com/PixlOne/logiops/wiki)
    
- [CIDs](https://github.com/PixlOne/logiops/wiki/CIDs)
    
- [Configuration](https://github.com/PixlOne/logiops/wiki/Configuration)
    
    - [Ignoring Devices](https://github.com/PixlOne/logiops/wiki/Configuration#ignoring-devices)
    - [Defining Devices](https://github.com/PixlOne/logiops/wiki/Configuration#defining-devices)
    - [Device Object](https://github.com/PixlOne/logiops/wiki/Configuration#device-object)
    - [name](https://github.com/PixlOne/logiops/wiki/Configuration#name)
    - [buttons](https://github.com/PixlOne/logiops/wiki/Configuration#buttons)
    - [Button Objects](https://github.com/PixlOne/logiops/wiki/Configuration#button-objects)
    - [cid](https://github.com/PixlOne/logiops/wiki/Configuration#cid)
    - [action](https://github.com/PixlOne/logiops/wiki/Configuration#action)
    - [dpi](https://github.com/PixlOne/logiops/wiki/Configuration#dpi)
    - [smartshift](https://github.com/PixlOne/logiops/wiki/Configuration#smartshift)
    - [on](https://github.com/PixlOne/logiops/wiki/Configuration#on)
    - [threshold](https://github.com/PixlOne/logiops/wiki/Configuration#threshold)
    - [default_threshold](https://github.com/PixlOne/logiops/wiki/Configuration#default_threshold)
    - [hiresscroll](https://github.com/PixlOne/logiops/wiki/Configuration#hiresscroll)
    - [hires](https://github.com/PixlOne/logiops/wiki/Configuration#hires)
    - [invert](https://github.com/PixlOne/logiops/wiki/Configuration#invert)
    - [target](https://github.com/PixlOne/logiops/wiki/Configuration#target)
    - [up](https://github.com/PixlOne/logiops/wiki/Configuration#up)
    - [down](https://github.com/PixlOne/logiops/wiki/Configuration#down)
    - [thumbwheel](https://github.com/PixlOne/logiops/wiki/Configuration#thumbwheel)
    - [divert](https://github.com/PixlOne/logiops/wiki/Configuration#divert)
    - [invert](https://github.com/PixlOne/logiops/wiki/Configuration#invert-1)
    - [left](https://github.com/PixlOne/logiops/wiki/Configuration#left)
    - [right](https://github.com/PixlOne/logiops/wiki/Configuration#right)
    - [proxy](https://github.com/PixlOne/logiops/wiki/Configuration#proxy)
    - [touch](https://github.com/PixlOne/logiops/wiki/Configuration#touch)
    - [tap](https://github.com/PixlOne/logiops/wiki/Configuration#tap)
    - [Actions](https://github.com/PixlOne/logiops/wiki/Configuration#actions)
    - [type](https://github.com/PixlOne/logiops/wiki/Configuration#type)
    - [None](https://github.com/PixlOne/logiops/wiki/Configuration#none)
    - [Keypress](https://github.com/PixlOne/logiops/wiki/Configuration#keypress)
    - [keys](https://github.com/PixlOne/logiops/wiki/Configuration#keys)
    - [Gestures](https://github.com/PixlOne/logiops/wiki/Configuration#gestures)
    - [gestures](https://github.com/PixlOne/logiops/wiki/Configuration#gestures-1)
    - [direction](https://github.com/PixlOne/logiops/wiki/Configuration#direction)
    - [threshold](https://github.com/PixlOne/logiops/wiki/Configuration#threshold-1)
    - [mode](https://github.com/PixlOne/logiops/wiki/Configuration#mode)
    - [NoPress](https://github.com/PixlOne/logiops/wiki/Configuration#nopress)
    - [OnRelease](https://github.com/PixlOne/logiops/wiki/Configuration#onrelease)
    - [OnInterval](https://github.com/PixlOne/logiops/wiki/Configuration#oninterval)
    - [OnThreshold](https://github.com/PixlOne/logiops/wiki/Configuration#onthreshold)
    - [Axis](https://github.com/PixlOne/logiops/wiki/Configuration#axis)
    - [action](https://github.com/PixlOne/logiops/wiki/Configuration#action-1)
    - [ToggleSmartShift](https://github.com/PixlOne/logiops/wiki/Configuration#togglesmartshift)
    - [ToggleHiresScroll](https://github.com/PixlOne/logiops/wiki/Configuration#togglehiresscroll)
    - [CycleDPI](https://github.com/PixlOne/logiops/wiki/Configuration#cycledpi)
    - [dpis](https://github.com/PixlOne/logiops/wiki/Configuration#dpis)
    - [sensor](https://github.com/PixlOne/logiops/wiki/Configuration#sensor)
    - [ChangeDPI](https://github.com/PixlOne/logiops/wiki/Configuration#changedpi)
    - [inc](https://github.com/PixlOne/logiops/wiki/Configuration#inc)
    - [sensor](https://github.com/PixlOne/logiops/wiki/Configuration#sensor-1)
    - [ChangeHost](https://github.com/PixlOne/logiops/wiki/Configuration#changehost)
    - [host](https://github.com/PixlOne/logiops/wiki/Configuration#host)
    - [Miscellaneous](https://github.com/PixlOne/logiops/wiki/Configuration#miscellaneous)
    - [workers](https://github.com/PixlOne/logiops/wiki/Configuration#workers)
    - [io_timeout](https://github.com/PixlOne/logiops/wiki/Configuration#io_timeout)
    
- [DBus Interface](https://github.com/PixlOne/logiops/wiki/DBus-Interface)
    
- [HIDPP 2.0](https://github.com/PixlOne/logiops/wiki/HIDPP--2.0)
    

##### Clone this wiki locally

## Footer

[](https://github.com/ "GitHub")©