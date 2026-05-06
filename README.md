# Vuzix Barcode SDK

## SDK Applicability
This is an SDK for interacting with Vuzix® smart glasses to enable barcode scanning. It is available
to developers writing software for Vuzix products.

This SDK provides a simple [Intent](https://developer.android.com/reference/android/content/Intent) 
based interface that launches Vuzix's embedded barcode scanning application and returns a single scan
result to your application.  This is a very useful mechanism that allows you to quickly implement a
scanner with almost no code, and no need for Camera permission in your application. It is recommended
for developers that need only an occasional barcode or 2D code (such as for login or configuration).

On legacy Vuzix products, this SDK enabled access to a proprietary barcode engine that provided
substantial improvements over other engines available at that time. In recent years there have been
substantial advances in the free engines, including Google
[ML Kit](https://developers.google.com/ml-kit/vision/barcode-scanning), and the proprietary engine
Vuzix had previously distributed via this SDK is no longer included.

SDK versions 1.0 through 1.71 provided two additional modes of operation that are supported on Vuzix
M300,  M400, M4000, Blade, Blade2, and Shield. These provided more control over the UI of the
scanner. The older SDK versions may still be used on those products, but using the additional two
modes of operation from SDK 1.x on newer Vuzix products including Vuzix LX1 is not supported. Only
the interfaces exposed in SDK version 2.0.0 and higher are supported in the latest Vuzix hardware.

Developers wanting a low-code implementation to quickly add barcodes to their application should
use this SDK. Developers wanting full control over the configuration of the scanner and the UI
presentation should integrate a third-party engine.

## Usage Instructions
This is a repository contains only binary artifacts. Although you may downlodad the .jar file directly, it is preferred to download it automatically using the gradle,
maven, sbt, or leiningen build system. Simplified instructions for this are available on [jitpack.io](https://jitpack.io/#com.vuzix/sdk-barcode)

Full documentation on installation and usage is available on [vuzix.com](https://www.vuzix.com) under Support > Developer center. Simply click the Knowledge Base for
the appropriate product and reference the section: "Working with the Barcode SDK."

For additional information, please refer to the [Vuzix Barcode SDK Javadocs](https://vuzix.github.io/sdk-barcode/javadoc/reference/classes.html).

## Legal
Use of the SDK is available to developers agreeing to the 
[VUZIX® SOFTWARE DEVELOPMENT KIT LICENSE AND CONFIDENTIALITY AGREEMENT](https://www.vuzix.com/pages/vuzix%C2%AE-software-development-kit-license-and-confidentiality-agreement)

[![](https://jitpack.io/v/com.vuzix/sdk-barcode.svg)](https://jitpack.io/#com.vuzix/sdk-barcode)
