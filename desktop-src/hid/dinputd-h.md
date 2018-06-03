---
Description: This section contains reference topics for the Dinputd.h header.
ms.assetid: C87F7308-D143-4268-A423-FFCC1CCB3AE4
title: Dinputd.h
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Dinputd.h

This section contains reference topics for the Dinputd.h header.

## In this section



| Topic                                                                   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|-------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**DIDEVICESTATE**](/windows/desktop/api/Dinputd/ns-dinputd-didevicestate)<br/>                       | The [**DIDEVICESTATE**](/windows/desktop/api/Dinputd/ns-dinputd-didevicestate) structure returns information about the state of a force feedback device. <br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [**DIDRIVERVERSIONS**](/windows/desktop/api/Dinputd/ns-dinputd-didriverversions)<br/>                 | The [**DIDRIVERVERSIONS**](/windows/desktop/api/Dinputd/ns-dinputd-didriverversions) structure is used by the DirectInput effect driver to report version information back to DirectInput. The semantics of the version numbers are left to the discretion of the device driver. The only requirement is that later versions have higher version numbers than earlier versions. <br/>                                                                                                                                                                                                                                                                                                                                                                                    |
| [**DIEFFECTATTRIBUTES**](/windows/desktop/api/Dinputd/ns-dinputd-dieffectattributes)<br/>             | The [**DIEFFECTATTRIBUTES**](/windows/desktop/api/Dinputd/ns-dinputd-dieffectattributes) structure describes the information contained in the "Attributes" value of the registry key for each effect that is supported by a force-feedback device. <br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [**DIFFDEVICEATTRIBUTES**](/windows/desktop/api/dinputd/ns-dinputd-diffdeviceattributes)<br/>         | The DIFFDEVICEATTRIBUTES structure describes the information contained in the "Attributes" value of the **OEMForceFeedback** registry key. <br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| [**DIFFOBJECTATTRIBUTES**](/windows/desktop/api/Dinputd/ns-dinputd-diffobjectattributes)<br/>         | The DIFFOBJECTATTRIBUTES structure describes the information contained in the "FFAttributes" value of the registry key for each "object" on a force-feedback device. If the "FFAttributes" value is absent, then the object is assumed not to support force feedback. <br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| [**DIHIDFFINITINFO**](/windows/desktop/api/Dinputd/ns-dinputd-dihidffinitinfo)<br/>                   | The [**DIHIDFFINITINFO**](/windows/desktop/api/Dinputd/ns-dinputd-dihidffinitinfo) structure is used by DirectInput to provide information to a HID force-feedback driver about the device it is being asked to control.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| [**DIJOYCONFIG**](/windows/desktop/api/Dinputd/ns-dinputd-dijoyconfig)<br/>                           | The DIJOYCONFIG structure contains information about a joystick's configuration. <br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| [**DIJOYTYPEINFO**](/windows/desktop/api/Dinputd/ns-dinputd-dijoytypeinfo)<br/>                       | The [**DIJOYTYPEINFO**](/windows/desktop/api/Dinputd/ns-dinputd-dijoytypeinfo) structure contains information about a joystick type. <br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| [**DIJOYUSERVALUES**](/windows/desktop/api/Dinputd/ns-dinputd-dijoyuservalues)<br/>                   | The [**DIJOYUSERVALUES**](/windows/desktop/api/Dinputd/ns-dinputd-dijoyuservalues) structure contains information about the user's joystick settings. <br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [**DIOBJECTATTRIBUTES**](/windows/desktop/api/Dinputd/ns-dinputd-diobjectattributes)<br/>             | The DIOBJECTATTRIBUTES structure describes the information contained in the "Attributes" value of the registry key for each "object" on a device. If the "Attributes" value is absent, then default attributes are used. <br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [**DIOBJECTCALIBRATION**](/windows/desktop/api/Dinputd/ns-dinputd-diobjectcalibration)<br/>           | The DIOBJECTCALIBRATION structure describes the information contained in the "Calibration" value of the registry key for each axis on a device.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [**IDirectInputEffectDriver**](/windows/desktop/api/Dinputd/nn-dinputd-idirectinputeffectdriver)<br/> | These three methods allow additional interfaces to be added to the DirectInputEffectDriver object without affecting the functionality of the original interface. <br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| [**IDirectInputJoyConfig8**](/windows/desktop/api/Dinputd/nn-dinputd-idirectinputjoyconfig8)<br/>     | **IDirectInputJoyConfig8** interface contains methods that allow hardware developers who are writing property sheets to write and read information to and from the registry. If you need to open registry keys, you should use the [**IDirectInputJoyConfig8::OpenConfigKey**](/windows/desktop/api/Dinputd/) and [**IDirectInputJoyConfig8::OpenTypeKey**](/windows/desktop/api/dinputd/nf-dinputd-idirectinputjoyconfig8-opentypekey) methods rather than opening registry keys directly. Using either of these methods ensures that the correct registry branch is opened. In addition, the **IDirectInputJoyConfig8** interface will be supported in future versions of DirectInput when the underlying registry data may be structured differently.<br/> |



 

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bhid\hid%5D:%20Dinputd.h%20%20RELEASE:%20%285/12/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")



