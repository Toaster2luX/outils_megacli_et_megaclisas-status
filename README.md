## Exécution
-----------------
$ ansible-playbook -i hosts playbooks/hwraid.yml
 
## Exécution sur une target
-----------------
$ ansible-playbook -i hosts playbooks/hwraid.yml -l "192.168.3.95"
 
### Source
-----------------
https://blog.izero.fr/ansible-installation-des-outils-megacli-et-megaclisas-status/

### Exemple
-----------------
$ sudo megaclisas-status

-- Controller information --
-- ID | H/W Model       | RAM    | Temp | BBU    | Firmware
c0    | PERC H710P Mini | 1024MB | 47C  | Good   | FW: 21.3.5-0002

-- Array information --
-- ID | Type   |    Size |  Strpsz | Flags | DskCache |   Status |  OS Path | CacheCade        |InProgress
c0u0  | RAID-5 |   6545G |   64 KB | RA,WB |  Default |  Optimal | /dev/sda | Type : Read Only |None

-- Disk information --
-- ID   | Type | Drive Model                       | Size     | Status          | Speed    | Temp | Slot ID  | LSI ID
c0u0p0  | HDD  | SEAGATE ST1200MM0007 IS06S3L0N06D | 1.090 TB | Online, Spun Up | 6.0Gb/s  | 28C  | [32:0]   | 0
c0u0p1  | HDD  | SEAGATE ST1200MM0007 IS06S3L0MPRD | 1.090 TB | Online, Spun Up | 6.0Gb/s  | 27C  | [32:1]   | 1
c0u0p2  | HDD  | SEAGATE ST1200MM0007 IS06S3L0MPGJ | 1.090 TB | Online, Spun Up | 6.0Gb/s  | 28C  | [32:2]   | 2
c0u0p3  | HDD  | SEAGATE ST1200MM0007 IS06S3L0N087 | 1.090 TB | Online, Spun Up | 6.0Gb/s  | 26C  | [32:3]   | 3
c0u0p4  | HDD  | SEAGATE ST1200MM0007 IS06S3L0MP7H | 1.090 TB | Online, Spun Up | 6.0Gb/s  | 28C  | [32:4]   | 4
c0u0p5  | HDD  | SEAGATE ST1200MM0007 IS06S3L0MASA | 1.090 TB | Online, Spun Up | 6.0Gb/s  | 26C  | [32:5]   | 5
c0u0p6  | HDD  | SEAGATE ST1200MM0007 IS06S3L0MP68 | 1.090 TB | Online, Spun Up | 6.0Gb/s  | 28C  | [32:6]   | 6

-- Unconfigured Disk information --
-- ID   | Type | Drive Model                       | Size     | Status              | Speed    | Temp | Slot ID  | LSI ID | Path
c0uXpY  | HDD  | SEAGATE ST1200MM0007 IS06S3L0MPHA | 1.090 TB | Hotspare, Spun Up   | 6.0Gb/s  | 27C  | [32:7]   | 7      | N/A
