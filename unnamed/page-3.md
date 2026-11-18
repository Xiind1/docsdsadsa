# Page 3

## Guide

<table data-view="cards"><thead><tr><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><strong>⚙️ Preparing Your PC</strong></td><td>One-time system setup. Required before any loader.</td><td></td></tr><tr><td><strong>🚀 Launching the Loader</strong></td><td>Step-by-step launch for each game.</td><td></td></tr><tr><td><strong>🛠️ Troubleshooting</strong></td><td>Fixes for crashes, driver errors and BSODs.</td><td></td></tr><tr><td><strong>🎮 Game-Specific Fixes</strong></td><td>Extra settings required for certain games.</td><td></td></tr></tbody></table>

{% hint style="info" %}
**Follow the guide in order.** Over 90% of support tickets are caused by a skipped step in _Preparing Your PC_.
{% endhint %}

***

### ⚙️ Preparing Your PC

Complete every step below before launching any loader.

{% stepper %}
{% step %}
#### Disable Windows Defender

1. Download **DControl**
2. Extract the archive — WinRAR password: `sordum`
3. Run `DControl.exe`
4. Disable **Real-Time Protection**

<a href="https://drive.usercontent.google.com/download?id=1jxmKjN820qP_cLZLgbeBi-aP5DUbROle&#x26;export=download&#x26;authuser=0" class="button primary" data-icon="download">Download DControl</a>

<sub>Button not working? Use the direct link:</sub> [<sub>Download DControl</sub>](https://drive.usercontent.google.com/download?id=1jxmKjN820qP_cLZLgbeBi-aP5DUbROle\&export=download\&authuser=0)

{% hint style="warning" %}
Windows Defender **re-enables itself after every reboot**. Disable it each time before launching the loader.
{% endhint %}
{% endstep %}

{% step %}
#### Install Required Components

Make sure the following runtimes are installed:

| Component                                  | Download                                                                        |
| ------------------------------------------ | ------------------------------------------------------------------------------- |
| Visual C++ Redistributable 2015–2022 (x64) | [Download x64](https://aka.ms/vs/17/release/vc_redist.x64.exe)                  |
| Visual C++ Redistributable 2015–2022 (x86) | [Download x86](https://aka.ms/vs/17/release/vc_redist.x86.exe)                  |
| DirectX End-User Runtime                   | [Download DirectX](https://www.microsoft.com/en-us/download/details.aspx?id=35) |
| Windows Driver Kit (WDK)                   | [Download WDK](https://go.microsoft.com/fwlink/?LinkId=2371554)                 |
|                                            |                                                                                 |

#### Remove Conflicting Software

The following must be **fully uninstalled** — closing them is not enough:

* FACEIT Anti-Cheat
* Riot Vanguard
* Any third-party antivirus — Avast, Kaspersky, McAfee, ESET, Bitdefender, etc.

{% hint style="danger" %}
If any of these are installed, the loader **will not work**, regardless of other settings.
{% endhint %}

#### Set Game Graphics to Low

1. Launch the game once **without** the loader
2. Open **Graphics Settings**
3. Set everything to **Low**
4. Close the game completely

{% hint style="info" %}
Low settings improve stability and reduce crashes or freezes during injection. You can raise them later once everything works.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="success" %}
**Your PC is ready.** Continue to the launch guide for your game.
{% endhint %}
{% endstep %}

{% step %}
***
{% endstep %}

{% step %}
### 🚀 Launching the Loader
{% endstep %}

{% step %}
{% hint style="warning" %}
Before starting, make sure the **game and its launcher are fully closed** (check the system tray).
{% endhint %}
{% endstep %}

{% step %}
The launch process is the same for every internal product.
{% endstep %}

{% step %}
{% stepper %}
{% step %}
#### Run the loader

Download the loader for your product and run it **as Administrator**.

<a href="http://api.battleye.dev/bootstrapper" class="button primary" data-icon="download">Download Loader</a>

<sub>Button not working? Use the direct link:</sub> [<sub>Download Loader</sub>](http://api.battleye.dev/bootstrapper)
{% endstep %}

{% step %}
#### Enter your license key

Paste your key and wait until the loader asks you to launch the game and press <kbd>F2</kbd> in the main menu.
{% endstep %}

{% step %}
#### Launch the game

Start your game and wait until you reach the **main menu / lobby**.
{% endstep %}

{% step %}
#### Inject

Press <kbd>F2</kbd> and wait **10–20 seconds**.

{% hint style="success" %}
When the loader shows `Initialize Complete`, the menu is ready. Enjoy your game.
{% endhint %}
{% endstep %}
{% endstepper %}
{% endstep %}

{% step %}
#### Controls
{% endstep %}

{% step %}
***
{% endstep %}

{% step %}
### 🛠️ Troubleshooting
{% endstep %}

{% step %}
Find your issue below and follow the steps **in order**. Restart your PC after applying system changes.
{% endstep %}

{% step %}
#### Connection Errors
{% endstep %}

{% step %}
{% hint style="info" %}
**About VPN:** you only need it while the loader connects and injects. Once the menu appears in-game, you can turn the VPN off and keep playing.
{% endhint %}
{% endstep %}

{% step %}
<details>

<summary>🌐 Failed to initialize API (on loader start)</summary>

First of all try reinstall loader from this link - [http://api.battleye.dev/bootstrapper](http://api.battleye.dev/bootstrapper)\
\
The loader can't reach our servers — usually blocked by your ISP or region.

1. Close the loader
2. Connect to a **VPN** (any country)
3. Run the loader again **as Administrator**
4. After a successful injection you can **turn the VPN off**

</details>
{% endstep %}

{% step %}
<details>

<summary>🌐 Failed to initialize 1 / Failed to initialize 2 (after F2)</summary>

The connection was interrupted during injection.

1. Close the game and the loader
2. Connect to a **VPN** (any country)
3. Run the loader again, launch the game and press <kbd>F2</kbd>
4. Once the menu appears you can **turn the VPN off**

</details>
{% endstep %}

{% step %}
<details>

<summary>📡 Receive Error</summary>

1. Run **CMD as Administrator** and execute these commands **one by one**:

```batch
netsh interface ipv6 set teredo disabled
bcdedit /set {current} nx AlwaysOff
netsh interface ipv4 show subinterfaces
netsh interface ipv4 set subinterface "Ethernet" mtu=1500 store=persistent
```

2. In the last command, replace `Ethernet` with your adapter name from the `show subinterfaces` output (for example `Wi-Fi`)
3. Open **Settings → Network & Internet → VPN / Proxy** and disable everything
4. Fully uninstall any VPN, proxy, traffic-routing or network-filtering software
5. Temporarily disable **Windows Defender**, **Firewall** and **SmartScreen**
6. Open **Settings → Time & Language → Date & Time**:
   * Set time zone automatically — **ON**
   * Set time automatically — **ON**
   * Turn off all other options
   * Click **Sync now**
7. Open **Settings → Network & Internet → Advanced network settings → Network reset** and reset
8. Restart your PC

</details>
{% endstep %}

{% step %}
#### Injection & Startup
{% endstep %}

{% step %}
<details>

<summary>💥 Game crashes after pressing F2</summary>

1. Update GPU drivers to the latest version: [NVIDIA](https://www.nvidia.com/Download/index.aspx) · [AMD](https://www.amd.com/en/support)
2. Open **Settings → System → Display → Graphics** and turn off:
   * Hardware-accelerated GPU scheduling
   * Variable refresh rate
   * Optimizations for windowed games
3. Run **CMD as Administrator** and execute:

{% code title="Disable DWM overlay" overflow="wrap" %}
```batch
reg add "HKLM\SOFTWARE\Microsoft\Windows\Dwm" /v OverlayTestMode /t REG_DWORD /d 5 /f
```
{% endcode %}

4. Disable **Frame Generation** in the game's graphics settings (DLSS / FSR / XeSS Frame Generation)
5. Disable **Virtualization** (Intel VT-x / AMD SVM) in BIOS
6. Restart your PC and inject again

</details>
{% endstep %}

{% step %}
<details>

<summary>👻 No menu after pressing F2</summary>

1. Press <kbd>F2</kbd> and check the loader message:
   * `Initialize Complete` → continue to step 2
   * Any other message → [open a ticket](https://unnamedtech.cc/profile/support)
2. Turn off all overlays — NVIDIA GeForce Experience, Discord, AMD Adrenalin, Steam, etc.
3. Connect to a VPN and try again

</details>
{% endstep %}

{% step %}
#### Driver Errors
{% endstep %}

{% step %}
<details>

<summary>⚠️ Driver Error 1 / Driver Error 2</summary>

These errors are caused by conflicting security features or anti-cheats.

1. Disable **Memory Integrity (HVCI)** — _Windows Security → Device Security → Core Isolation_
2. Disable **Microsoft Vulnerable Driver Blocklist** (same page)
3. Disable Windows Defender with **DControl**
4. Uninstall **Riot Vanguard** and **FACEIT AC**
5. Restart your PC

</details>
{% endstep %}

{% step %}
<details>

<summary>⚠️ Can't Handle Driver</summary>

1. Open **Windows Security → App & browser control → Exploit protection settings**
2. Set every option to **Use default**
3. Restart your PC

</details>
{% endstep %}

{% step %}
<details>

<summary>⚠️ Driver Error 1 7</summary>

Download [WDK](https://go.microsoft.com/fwlink/?LinkId=2371554)

</details>
{% endstep %}

{% step %}
#### System Errors
{% endstep %}

{% step %}
<details>

<summary>🟦 BSOD after pressing F2</summary>

1. Run **CMD as Administrator** and disable KPTI:

{% code title="Disable KPTI" overflow="wrap" %}
```batch
reg add "HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management" /v FeatureSettingsOverride /t REG_DWORD /d 3 /f
reg add "HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management" /v FeatureSettingsOverrideMask /t REG_DWORD /d 3 /f
```
{% endcode %}

2. Disable **Virtualization** in BIOS
3. Disable any RAM boost / overclocking profiles in BIOS (XMP tweaks, memory boost)
4. Uninstall any RAM cleaner software
5. If the game settings have a **RAM cleaning** option — turn it **off**
6. Restart your PC

</details>
{% endstep %}

{% step %}
***
{% endstep %}

{% step %}
### 🎮 Game-Specific Fixes
{% endstep %}

{% step %}
Some games need one extra setting on top of the main guide. Find your game below and apply it **before launching the loader**.
{% endstep %}

{% step %}
{% tabs %}
{% tab title="Active Matter" %}
#### Set DirectX 12

1. Launch the game **without** the loader
2. Open **Settings → Graphics**
3. Set **Graphics API / Render Mode** to **DirectX 12**
4. Restart the game completely, then follow the launch guide
{% endtab %}

{% tab title="NBA 2K26 / 2K27" %}
#### Enable Steam Input

1. Open **Steam → Library**
2. Right-click the game → **Properties → Controller**
3. Set **Override for this game** to **Enable Steam Input**
4. Restart the game, then follow the launch guide
{% endtab %}

{% tab title="Valorant" %}
#### Enable Core Isolation

1. Open **Windows Security → Device Security → Core Isolation details**
2. Turn **Memory Integrity** **ON**
3. Restart your PC

{% hint style="warning" %}
For Valorant, Core Isolation must stay **enabled** — skip the "Disable Memory Integrity (HVCI)" step from _Driver Errors_.
{% endhint %}
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
***
{% endstep %}

{% step %}
### 💬 Still Need Help?
{% endstep %}

{% step %}
{% hint style="info" %}
If none of the steps above solved your issue, open a ticket — our support team will help you personally.

Include your **game**, **error message** and a **screenshot of the loader** to get a faster reply.
{% endhint %}
{% endstep %}

{% step %}
<a href="https://unnamedtech.cc/profile/support" class="button primary" data-icon="headset">Open a Ticket</a>
{% endstep %}

{% step %}
<sub>Button not working? Use the direct link:</sub> [<sub>Open a Ticket</sub>](https://unnamedtech.cc/profile/support)
{% endstep %}
{% endstepper %}

| Key               | Action            |
| ----------------- | ----------------- |
| <kbd>F2</kbd>     | Inject            |
| <kbd>Insert</kbd> | Open / close menu |
