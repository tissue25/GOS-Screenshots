# Explanation of 2-factor fingerprint unlock feature

## Explanation

One of the **flagship features** in GrapheneOS is the 2-factor fingerprint unlock. While the name of this feature may sound confusing at first, in simple words, it's a feature that lets you setup a disk encryption passcode and user passcode separately on a mobile device. For convenience, traditional phones usually only require one password, but the idea here was to verify the owner of the device, not to support a solid encryption system.

2-factor fingerprint unlock is different from such approach, as users can setup a passcode (usually a passphrase) for unlocking the BFU state device, and a more convenient PIN-based unlocking method for AFU states. 

**Traditional mobile phones:**
- One unlock passcode (PIN, passcode, pattern, etc.)

**GrapheneOS (Without 2FF):**
- One unlock passcode (PIN, passcode)

**GrapheneOS (With 2FF):**
- BFU passcode: (passphrase, etc.)
- AFU passcode: (fingerprint + PIN)

However, the necessity of setting up the 2-factor fingerprint unlock depends on whether you trust the secure element in Pixel devices. 


## 2FF Setup

1. In the Settings app, enter _Security & privacy > Device unlock > Screen lock > Choose a new screen lock_

2. Click _Password_ and setup a new passcode (a passphrase is recommended)

3. Return to _Security & privacy > Device unlock_, and enter _Fingerprint Unlock_

4. Setup the fingerprint if you haven't.

5. Enable _Use for screen unlocking_

6. Enter _Second factor PIN_

7. Setup the 2FF PIN.

<img alt="Home" src="https://raw.githubusercontent.com/tissue25/GOS-Screenshots/refs/heads/main/2-factor%20fingerprint%20unlock%20EXPLANATION/2FF.png" width="300">


Note that duress password can be used on the 2FF PIN screen too. 

**Keywords:**
- Passcode: A key required for unlocking.
- Password: A passcode consisted of alphabets, numbers, and special characters.
- Passphrase: A password consisted of words unlike password, for a longer and more memorable purpose. 
- PIN: Personal Identification Number. A passcode consisted of numbers.
- BFU: Before-First-Unlock, an encrypted state after the device reboot.
- AFU: After-First-Unlock.

More details can be found here:
https://discuss.grapheneos.org/d/18585-2-factor-fingerprint-unlock-feature-is-now-fully-implemented
https://grapheneos.org/features#two-factor-fingerprint-unlock


