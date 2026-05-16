<div align="center">

# Open QWear

Powerful AI software runs with Qwen/Quark S1/G1.

</div>

> **Disclaimer**
>  
>   *"Open QWear" is an independent open-source project and is not affiliated with, endorsed by, or officially associated with Alibaba, Qwen, Quark, or their respective organizations.*  
>   *The "Qwen" name, logo <img src="https://img.shields.io/badge/-6A5CFF?logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGZpbGw9IndoaXRlIiB2aWV3Qm94PSIwIDAgMTAyNCAxMDI0Ij48cGF0aCBkPSJNNDA2LjUgMTYwLjljLTEuMS41LTIuNyAxLjctMy42IDIuNy00LjIgNC43LTg3IDE1MS4yLTg3LjUgMTU0LjktLjQgMi41IDIuMSA3LjUgMTUuNyAzMC41IDguOSAxNS4xIDE4LjkgMzIuMSAyMi4yIDM3LjcgNC41IDcuNiA2LjkgMTAuNiA5LjMgMTEuOCAyLjggMS4zIDI0LjUgMS41IDE5Mi4xIDEuNSAxODEuOSAwIDE4OC45LS4xIDE5MS44LTEuOSA0LjMtMi42IDQ1LjUtNzQuNCA0NS41LTc5LjMgMC0zLjMtMTEuNi0yNC41LTM5LjQtNzEuNi0xLjctMy00LjMtNi01LjgtNi44LTIuMy0xLjItMTgtMS40LTk3LjYtMS40LTg5LjEgMC05NS0uMS05Ni41LTEuOC0xLjItMS40LTI1LjItNDIuMy0zOC40LTY1LjctMS45LTMuMy00LjUtNy4xLTUuOS04LjVsLTIuNC0yLjUtNDguOC0uMmMtMjYuOC0uMS00OS42LjItNTAuNy42TTIxMi40IDM2MC40Yy0zLjMgMS41LTQuNSAzLjQtMzMgNTMuNi0xNi40IDI4LjktMTYuMyAyOC41LTkuMyA0MCA0LjkgOC4xIDIyLjIgMzcuMiAzNi40IDYxLjUgNC45IDguMiAxOC4yIDMwLjggMjkuNyA1MC4yIDEyLjggMjEuNiAyMC44IDM2LjIgMjAuOCAzNy44IDAgMy4zLS44IDQuOS0yMSA0MC41LTIzLjkgNDIuNC0yNCA0Mi41LTI0IDQ1LjcgMCAyLjggNi4yIDE0LjEgMzIuMiA1OC4zIDkuNCAxNS45IDEyLjEgMTkuOCAxNC45IDIxLjIgMy4yIDEuNyA5LjYgMS44IDkyLjIgMS44IDk0LjkgMCA5My4zLjEgOTYuMy00LjdDNDU3LjEgNzUxIDQ5MCA2OTEuOCA0OTAgNjkwYzAtMS4zLTMuMS03LjgtNi45LTE0LjQtMTcuNC0zMC40LTQwLjUtNzAuNC00OC42LTg0LjEtNC44LTguMy0xNy0yOS4yLTI3LTQ2LjUtMTkuOS0zNC40LTY4LjEtMTE3LjQtODcuMi0xNTAtNi42LTExLjMtMTMuNC0yMy4xLTE1LjMtMjYuMy01LjctMTAuMS0zLjQtOS43LTQ5LjUtOS43LTMxLjIuMS00MC43LjQtNDMuMSAxLjRtNDY2LjQgNzQuMWMtMy4zIDEuOC0yLjcuOS00MiA3MC41LTg0LjcgMTQ5LjktMTUxLjIgMjY4LjctMTUyLjEgMjcxLjctLjggMi43LS43IDQuMS43IDcuMSA0IDguNSA0My4yIDc0LjkgNDUuNyA3Ny41bDIuNyAyLjdoOTEuOGwzLjItMi44YzEuOS0xLjYgOS40LTEzLjYgMTguOC0zMC4yIDI0LjEtNDIuMyA3MC4zLTEyMy45IDczLjctMTMwIDEuNi0zIDQuMS03IDUuNC04LjhsMi40LTMuMmg0OC43YzQ0LjQgMCA0OS0uMiA1Mi4yLTEuOCAyLjktMS40IDUuMy00LjkgMTQuNy0yMS4yIDMwLjgtNTMuMSAzNC4zLTU5LjYgMzQuMy02M3MtMy41LTkuOC0yNy41LTUwLjVjLTYuMi0xMC41LTIzLjUtNDAuMi0zOC41LTY2LTE1LTI1LjktMjguNS00OC40LTMwLjEtNTBsLTIuOS0zLTQ5LjMtLjJjLTQxLjYtLjItNDkuNiAwLTUxLjkgMS4yIi8+PC9zdmc+" align="absmiddle"> , and related branding assets are trademarks or copyrighted materials of the Qwen team and their respective owners. They are used in this project for identification and compatibility purposes only.*

## What Had We Done? (May 16, 2026)

| Component | Status |
| - | - |
| Overall Architecture | The architecture of the Qwen/Quark S1/G1 has been identified as `bes_2800_RTOS + qcom_ar1_android`. |
| `bes_2800_RTOS` | We are now able to send and receive **custom BLE GMA commands** for `bes_2800_RTOS`. |
| `qcom_ar1_android` | We are now able to obtain a **root shell with seccomp disabled** on `qcom_ar1_android`. |
| ❌ Display | We are currently unable to directly control the S1 display. The display appears to be connected directly to `bes_2800_RTOS`, and we have not yet been able to establish a video stream, image output, or toast rendering through either `qcom_ar1_android` or custom BLE GMA payloads targeting `bes_2800_RTOS`. |
| ❌ RTOS Firmware  | The ROM binary of `bes_2800_RTOS` for the S1 has been extracted, but it cannot currently be decrypted due to high-entropy encryption. |

## Detailed Architecture Observations

`qcom_ar1_android` in the Qwen/Quark S1/G1 appears to serve only on these really limited purposes:

**Camera**  
  Camera operations, ISP processing, and image stabilization functionality appear to be routed through the `qcom_ar1_android` and handled using the Qualcomm imaging stack and AliGenie custom image stabilization pipeline.

**AliPay Payment Security**  
  Alipay payment functionality appears to rely on Qualcomm TrustZone technology within the `qcom_ar1_android` to ensure secure payment processing.

Bluetooth communication were on `bes_2800_RTOS`.

When the `qcom_ar1_android` is powered off, `bes_2800_RTOS` continues running independently and showing **Camera not ready** .

## Roadmap
```
Custom QWear App
├─ Reroute AI requests to custom LLM providers
├─ Implement minimal on-device (Phone Companion)
│  AI agent functionality
└─ Reimplement all functionality
   of QwenWear (com.alibaba.wow)

Custom Qwen/Quark S1/G1 Firmware
└─ Waiting for further updates...
```
