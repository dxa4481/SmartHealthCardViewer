# Smart Vaccine Card Reader

[security.love/smarthealthcardviewer/](https://security.love/SmartHealthCardViewer/)

![example image](https://i.imgur.com/3DsGoKU.png)

## What are SMART Health Cards?

Smart Health is an [open standard](https://spec.smarthealth.cards/) that can be used to cryptographically attest to healthcare records

California has adopted this system and you can download your healthcard [here](https://myvaccinerecord.cdph.ca.gov/) if you got a COVID19 vaccine in the state of California

Here's more info about them from the [EFF](https://www.eff.org/deeplinks/2021/06/decoding-californias-new-digital-vaccine-records-and-potential-dangers)

## How can I view the data is in my SMART Health Card?

They're kind of a pain because they're encoded 3 or 4 times over, it almost feels like a CTF

[smarthealth.cards](https://smarthealth.cards) does have a portal that allows you to scan a smart healthcard, but this portal uploads your card to a server, and requirs you grant webcam access to the website to scan your card.

This repo contains code that staticly client side reads a smart card and mirrors the data back to you. [It's hosted here](https://security.love/SmartHealthCardViewer/)

Note: this site does not validate the card, and does not check the signature at all. It's just a data viewer.

## Why should you care?

If you get asked to scan your smart card, you should know what data you're giving up.

## What else?

It's likely other scanners are going to be lazy like me and not validate the signature of the healthcare provider. This could lead to forged smart cards

## Anything else?

Careful where you post your smart card, I'm not sure I'd even recommend posting it on my static client side site, even though it's all client side, you'd have to take my word at that.


Follow me on twitter [@insecureNature](https://twitter.com/InsecureNature)
