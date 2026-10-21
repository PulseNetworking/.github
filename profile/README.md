<p align="center">
  <img src="https://raw.githubusercontent.com/PulseNetworking/branding/refs/heads/main/dest/pulse-banner-2560x640.png" width="100%">
</p>

<p align="center">
  <a href="https://github.com/pulsenetworking/pulse"><img src="https://img.shields.io/badge/Unity-6000.0%2B-0B0F14?logo=unity&amp;logoColor=white" alt="Unity 6000.0 or newer"></a>
  <a href="https://github.com/pulsenetworking/pulse/blob/master/Packages/com.pulsenetworking.pulse/LICENSE.md"><img src="https://img.shields.io/badge/license-MIT-22D3EE" alt="MIT license"></a>
</p>

<p align="center">
  <a href="#packages">Packages</a> · <a href="#get-started">Get started</a> · <a href="#contributing">Contributing</a>
</p>

**Pulse** is open source netcode for Unity 6, for hosted or dedicated server games, with the networking boilerplate generated for you.
- **Write gameplay, not plumbing.** The underlying logic for synced communication is done for you. **Synced Variable**s are filled out via a source generator.
- **Feels right at any ping.** Client prediction, lag compensation and interest management are built in.
- **Reaches every player.** UDP, TCP or WebSockets, and a relay or TURN server for hosts behind NAT.

## Packages
| Package | Adds |
|---|---|
| [`com.pulsenetworking.pulse`](https://github.com/pulsenetworking/pulse/tree/master/Packages/com.pulsenetworking.pulse) | Transports, serialization, netcode. Everything else builds on it. |
| [`com.pulsenetworking.pulse.relay`](https://github.com/pulsenetworking/pulse/tree/master/Packages/com.pulsenetworking.pulse.relay) | Relay and TURN, for hosts behind NAT |
| [`com.pulsenetworking.pulse.lagcompensation`](https://github.com/pulsenetworking/pulse/tree/master/Packages/com.pulsenetworking.pulse.lagcompensation) | Hit checks against where targets were on the shooter's screen |
| [`com.pulsenetworking.pulse.xr`](https://github.com/pulsenetworking/pulse/tree/master/Packages/com.pulsenetworking.pulse.xr) | Networked XR rigs and grabbables |
| [`com.pulsenetworking.pulse.diagnostics`](https://github.com/pulsenetworking/pulse/tree/master/Packages/com.pulsenetworking.pulse.diagnostics) | An in-game overlay with traffic, ping and state sizes |
| [`com.pulsenetworking.pulse.examples`](https://github.com/pulsenetworking/pulse/tree/master/Packages/com.pulsenetworking.pulse.examples) | Example scenes to start from |

## Get started
Pulse needs **Unity 6000.0 or newer** and **[UniTask](https://github.com/Cysharp/UniTask)**.

1. Add UniTask to `Packages/manifest.json`:
   ```json
   "com.cysharp.unitask": "https://github.com/Cysharp/UniTask.git?path=src/UniTask/Assets/Plugins/UniTask"
   ```
   **Or** in Package Manager, choose **+ › Add package from git URL** and enter:
   ```
   https://github.com/Cysharp/UniTask.git?path=src/UniTask/Assets/Plugins/UniTask
   ```
   
3. In Package Manager, choose **+ › Add package from git URL** and enter:
   ```
   https://github.com/pulsenetworking/pulse.git?path=Packages/com.pulsenetworking.pulse
   ```

## Contributing
Bug reports, ideas and pull requests are all welcome on [the issue tracker](https://github.com/pulsenetworking/pulse/issues). Pulse is [MIT licensed](https://github.com/pulsenetworking/pulse/blob/master/Packages/com.pulsenetworking.pulse/LICENSE.md).
