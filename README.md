<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/770bda67-782c-4ad4-bb54-b54b1c90c6bc" />



# GoAhead Museum – Research Dataset

This repository is a **catalog of embedded GoAhead / jhttpd web server binaries** collected from router and IoT firmware.  
The aim is to preserve these binaries as a **historical research dataset**, supporting the study of `goform`-based web servers, their variants, and their security issues.

---

## Purpose

* Provide researchers and practitioners with reference samples of GoAhead and related forks.  
* Encourage contributions of additional binaries for comparative analysis.  
* Support long-term study of how embedded web stacks evolve and eventually disappear.

---


## Dataset Format

Each contributed binary should be accompanied by metadata in the table format below.

| Sample ID             | Vendor / Model            | Firmware Ver.                     | Variant          | Link                                                                 |
| --------------------- | ------------------------- | --------------------------------- | ---------------- | -------------------------------------------------------------------- |
| jhttpd.NR500.EA       | NR500-EA                  | RG500UEAABxCOMSLICv3.4.2731.16.43 | jhttpd fork      | [link](https://github.com/actuator/DEFCON-33/blob/main/jhttpd-Model-NR500-EA-Firmware-RG500UEAABxCOMSLICv3-4-2731-16-43) |
| jhttpd.dionlink.M7628N| Tuoshi/Dionlink LT15D & LT21B 4G Wi-Fi | v1.0.1802.10.08.P4                | jhttpd fork      | [link](https://github.com/actuator/DEFCON-33/blob/main/jhttpd-dionlink-M7628NNxlSPv2xUI_v1-0-1802-10-08_P4) |
| kthy_topsw_goahead.topsw.GC111      | KTHY TopSW GC111-GL-LM321 | V3.0.20191211                     | OEM GoAhead fork | [link](https://github.com/actuator/DEFCON-33/blob/main/kthy_topsw_goahead_GC111-GL-LM321_V3.0_20191211) |
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

This dataset can help with:

* **Static Analysis** – compare different forks to trace patching and code reuse.  
* **Fuzzing** – build harnesses for legacy binaries to explore attack surfaces.  
* **Vulnerability Lineage** – map how known flaws persist or reappear across vendors.  
* **Decommission Tracking** – measure when (or if) GoAhead-based stacks vanish from production firmware.  

---

## Contributing

To contribute:

1. Upload the binary file.  
2. Add a row to the dataset table with the required metadata.  
3. Submit a pull request.  

All contributions will help expand the coverage of the GoAhead ecosystem and support future research.

---

## References

* [Examples of jhttpd/GoAhead forks](https://github.com/actuator/DEFCON-33)
