<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/770bda67-782c-4ad4-bb54-b54b1c90c6bc" />

# GoAhead Museum – Research Dataset

This repository is a **living archive of embedded GoAhead / jhttpd web server binaries** collected from router and IoT firmware images.  
It exists to **preserve historically significant embedded web stacks** and make them easily accessible for security research, reverse engineering, and long-term study.

GoAhead and its forks powered countless low-cost routers, access points, cameras, and IoT devices from the late 1990s through the 2010s. They introduced the `/goform` pattern for handling web requests, which became a de facto standard in many OEM firmware packages. As devices age out and firmware images disappear, this codebase — and its vulnerabilities — are at risk of being lost to history.  

---

## Purpose

* **Historical Preservation** – provide researchers with reference samples of GoAhead and related forks before they disappear from vendor sites.  
* **Security Research** – offer a centralized resource to compare implementations, patch histories, and vulnerability trends.  
* **Education** – show students and professionals how embedded web stacks evolved and how their security models worked (or failed).  
* **Collaboration** – encourage contributions of additional binaries for comparative analysis.  

---

## Dataset Format

Each contributed binary is stored with accompanying metadata.  
This allows researchers to understand the firmware context and track lineage across vendors and versions.

| Sample ID             | Vendor / Model            | Firmware Ver.                     | Variant          | Link                                                                 |
| --------------------- | ------------------------- | --------------------------------- | ---------------- | -------------------------------------------------------------------- |
| jhttpd.NR500.EA       | NR500-EA                  | RG500UEAABxCOMSLICv3.4.2731.16.43 | jhttpd fork      | [link](https://github.com/actuator/DEFCON-33/blob/main/jhttpd-Model-NR500-EA-Firmware-RG500UEAABxCOMSLICv3-4-2731-16-43) |
| jhttpd.dionlink.M7628N| Tuoshi/Dionlink LT15D & LT21B 4G Wi-Fi | v1.0.1802.10.08.P4                | jhttpd fork      | [link](https://github.com/actuator/DEFCON-33/blob/main/jhttpd-dionlink-M7628NNxlSPv2xUI_v1-0-1802-10-08_P4) |
| kthy_topsw_goahead.topsw.GC111 | KTHY TopSW GC111-GL-LM321 | V3.0.20191211                     | OEM GoAhead fork | [link](https://github.com/actuator/DEFCON-33/blob/main/kthy_topsw_goahead_GC111-GL-LM321_V3.0_20191211) |
| webserver.KuWFi.AC900 | KuWFi AC900               | V1.0.13                           | OEM GoAhead fork | [link](https://github.com/actuator/DEFCON-33/blob/main/webserver-KuWFi-AC900_FW_V1_0_13) |
| goahead.vendorRedacted.2.2.9 | Redacted | V2.2.9  | OEM GoAhead fork | [link](https://github.com/actuator/goform/blob/main/goahead.vendorRedacted-Ver-2.2.9.bin) |

---

## Metadata Fields

* **Sample ID** – filename in the repository.  
* **Vendor / Model** – hardware source device.  
* **Firmware Ver.** – vendor firmware version string.  
* **Variant** – GoAhead / jhttpd / OEM fork.  
* **Link** – reference to the hosted binary in this repo.  

---

## Research Directions

This dataset enables:

* **Static Analysis** – compare forks to trace patching, hard-coded credentials, and code reuse.  
* **Dynamic/Fuzz Testing** – build harnesses to explore attack surfaces of legacy binaries.  
* **Vulnerability Lineage** – map how known flaws persisted or reappeared across vendors.  
* **Decommission Tracking** – measure when GoAhead-based stacks vanished from production firmware.  
* **Teaching Material** – provide real embedded targets for labs and courses in security or reverse engineering.  

---

## Contributing

We welcome new binaries, metadata improvements, and analysis write-ups. To contribute:

1. Upload the binary file.  
2. Add a row to the dataset table with the required metadata.  
3. Submit a pull request or open an issue to discuss.  

All contributions help expand the coverage of the GoAhead ecosystem and support future research.

---

## Ethical Note

These binaries are provided **for research and educational purposes only**.  
They are not meant to encourage unauthorized access or exploitation of live systems.  

---

## References & Related Work

* [Examples of jhttpd/GoAhead forks](https://github.com/actuator/DEFCON-33)  
* [GoAhead WebServer overview (old upstream site)](https://web.archive.org/web/*/http://embedthis.com/goahead/)  

---

