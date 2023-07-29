# Storage Device Cables

## Integrated Drive Electronics (IDE)

[IDE (Integrated Drive Electronics)](https://www.techtarget.com/searchstorage/definition/IDE) is an electronic interface standard that defines the connection between a [bus](https://www.techtarget.com/searchstorage/definition/bus) on a computer's [motherboard](https://www.techtarget.com/whatis/definition/motherboard) and the computer's disk [storage](https://www.techtarget.com/searchstorage/definition/storage) device, enabling them to communicate with each other. At one time, most computers included at least one IDE interface built into the motherboard. The interface provided a 40-pin connector for attaching an IDE hard disk drive ([HDD](https://www.techtarget.com/searchstorage/definition/hard-disk-drive)) to the computer. A flat ribbon cable connected the drive to the motherboard by attaching to the IDE interfaces on the computer and HDD. The IDE interface was originally based on the IBM PC [Industry Standard Architecture](https://www.techtarget.com/searchwindowsserver/definition/ISA-Industry-Standard-Architecture) 16-bit bus standard, but it has since been implemented in computers that use other bus standards.

n November 1990, the American National Standards Institute ([ANSI](https://www.techtarget.com/searchdatacenter/definition/ANSI)) standardized the IDE technology, referring to it as Advanced Technology Attachment (ATA). The ATA standard is maintained by the T13 Committee of the International Committee on Information Technology Standards, an ANSI-accredited forum for creating technology standards.

The IDE interface standard grew out of the effort to combine a storage controller and the storage disk into a single unit. Before that, controllers and disks were implemented as separate devices, often built by different manufacturers. Not only did this result in integration issues, but the distance between the two could impact performance.

## Serial Advanced Technology Attachment (SATA)

Serial ATA (Serial Advanced Technology Attachment or SATA) is a command and transport protocol that defines how data is transferred between a computer's motherboard and mass storage devices, such as hard disk drives (HDDs), optical drives and solid-state drives (SSDs). As its name implies, SATA is based on serial signaling technology, where data is transferred as a sequence of individual bits.

The Serial ATA International Organization (SATA-IO) oversees the development of the technical specification. SATA specifies a transfer format and a wiring arrangement. It succeeded Parallel ATA ([PATA](https://www.techtarget.com/whatis/definition/Parallel-ATA-Parallel-Advanced-Technology-Attachment-or-PATA)) as the communications interface for most new computer systems. Those systems also usually support serial-attached SCSI ([SAS](https://www.techtarget.com/searchstorage/definition/serial-attached-SCSI)) and non-volatile memory express ([NVMe](https://www.techtarget.com/searchstorage/feature/The-present-and-likely-future-of-the-NVMe-protocol)) communication protocols.

### SATA vs PATA

When [comparing SATA and PATA](https://www.techtarget.com/searchstorage/tip/PATA-and-SATA-The-evolution-of-disk-standards), a serial connection requires fewer wires and results in a clearer signal than a parallel connection. This makes serial signals suitable for transmitting data over long distances.

A parallel signal is synchronous and requires a wider data bus. Multiple bits are sent simultaneously across different wires that are housed in the same cable. A clocking signal synchronizes the timing between the different channels. As a result, parallel transmission is better suited to shorter distances to avoid signal interference. The multiple wires that parallelism needs also makes it slightly more costly than serial transmission.

SATA offers several advantages compared with the IDE-based PATA standard developed in the 1980s. These advantages include the following:

- **Full-duplex performance.** Most notably, PATA is a [half-duplex](https://www.techtarget.com/searchnetworking/definition/half-duplex) transmission, making it unable to simultaneously receive and transmit data. This contrasts with SATA's [full-duplex](https://www.techtarget.com/searchnetworking/definition/full-duplex) performance.  
	- PATA drives deliver data bits simultaneously across a single ribbon cable that's 40-pin wide. The SATA standard defines a SATA cable with two pairs of differential wires, three ground pins and a separate power connector. One pair of wires transfers data and one pair receives data. Capping each end of the SATA conductors is an 8-millimeter wafer connector.
- **No resource contention.** SATA drives contain an independent computer host bus to eliminate [resource contention](https://www.techtarget.com/whatis/definition/resource-contention).
- **Faster throughput.** SATA transfers data one bit at a time between a drive and its host, using a seven-pin data cable and 15-pin drive power connector cable. The SATA cable results in a higher signaling rate, which corresponds to faster data throughput.
- **Design flexibility.** The SATA cables also offer flexible design in the physical layout of a system. The cables extend up to 39 inches, more than twice the length of the 18-inch ribbon cables required for conventional PATA hard drives. That gives system designers more leeway on where a drive can be mounted in a chassis. The narrow width of SATA cables also increases air flow within computers.
- **Additional features.** Older SATA drives are equipped with [jumpers](https://www.techtarget.com/whatis/definition/jumper) to enable additional features. A jumper is a rectangular plastic connector that creates a circuit when slid across two pins. The circuit activates and deactivates certain preprogrammed settings in a computer's [BIOS](https://www.techtarget.com/whatis/definition/BIOS-basic-input-output-system) or [Unified Extensible Firmware Interface](https://www.techtarget.com/whatis/definition/Unified-Extensible-Firmware-Interface-UEFI), such as regulating CPU speed, signal voltage and troubleshooting.  
	- The jumper technology is a holdover from IDE-based disk drives. They are seldom needed with computers made after 2002. One exception is using jumpers to slow down newer drives, enabling them to more efficiently use earlier versions of the SATA hardware interface. There is a risk in this, however, as incorrect jumper settings will hinder device detection as drives are added or swapped out.  

Using fewer [conductors](https://www.techtarget.com/whatis/definition/conductor) reduces the risk of [crosstalk](https://www.techtarget.com/searchnetworking/definition/crosstalk) and electromagnetic interference with SATA. The signal voltage is much lower as well: 250 millivolts for SATA vs. 5 volts for PATA.

## External SATA (eSATA)

When first conceived, SATA was intended as an internal mechanism to improve the performance of storage in consumer PCs. The need to extend that performance outside the chassis led to development of the External Serial Advanced Technology Attachment ([eSATA](https://sata-io.org/developers/sata-ecosystem/esata)).

SATA-IO developed eSATA as a variation of the SATA specification, using the same pins and protocol to ensure consistent performance. This allowed SATA storage devices to be connected externally to the computer's motherboard. The process uses a rugged power connector and two meters of shielded cables to transfer data between external devices and internal storage. SATA-IO claims eSATA transfers data up to six times faster than the USB 2.0 or IEEE 1394 interface.

A single eSATA port could be attached to an external SATA chassis to expand storage and build a RAID array. Video editing, audio production and data backup are some common use cases for eSATA drives. However, eSATA has limits. Many older SATA controllers and drives do not support the hot-swap capability that the external interface needs.

## FireWire

[IEEE 1394, commonly known as FireWire](https://www.lifewire.com/what-is-firewire-2625918), is a standard connection type for many electronic devices such as digital video cameras, printers and scanners, [external hard drives](https://www.lifewire.com/what-is-an-external-drive-2625867), and other peripherals. The terms IEEE 1394 and FireWire usually refer to the types of cables, ports, and connectors used to connect these types of external devices to computers.

It uses a six-pin connector and can transfer data at 100, 200, or 400 Mbps depending on the FireWire cable used on cables as long as 4.5 meters. These data transfer modes are commonly called _S100, S200,_ and _S400_. In the late 2000s, _FireWire S1600_ and _S3200_ came out. They supported transfer speeds as fast as 1,572 Mbps and 3,145 Mbps, respectively. However, so few of these devices were released that they shouldn't even be considered part of the timeline of FireWire development.

In 2011, Apple began replacing FireWire with the much faster [Thunderbolt](https://www.lifewire.com/what-is-thunderbolt-832713) and, in 2015, at least on some of their computers, with USB 3.1 compliant [USB-C](https://www.lifewire.com/usb-c-4149490) ports. The most recent USB standard is USB4, which supports transfer speeds as high as 40,960 Mbps. It's much faster than the 800 Mbps that FireWire supports. Another advantage that USB has over FireWire is that USB devices and cables are usually cheaper than their FireWire counterparts, no doubt due to how popular and mass-produced USB devices and cables have become.

## Small Computer System Interface (SCSI)

[SCSI](https://www.techtarget.com/searchstorage/definition/SCSI) (pronounced SKUH-zee and sometimes colloquially known as "scuzzy"), the Small [Computer System](https://www.techtarget.com/searchwindowsserver/definition/system) Interface, is a set of American National Standards Institute ([ANSI](https://www.techtarget.com/searchdatacenter/definition/ANSI)) standard electronic interfaces that allow personal computers ([PCs](https://www.techtarget.com/whatis/definition/personal-computer-PC)) to communicate with peripheral hardware such as [disk drives](https://www.techtarget.com/searchstorage/definition/hard-disk-drive), [tape drives](https://www.techtarget.com/searchstorage/definition/tape-drive), [CD-ROM](https://www.techtarget.com/searchstorage/definition/compact-disc) drives, [printers](https://www.techtarget.com/whatis/definition/printer) and [scanners](https://www.techtarget.com/whatis/definition/scanner) faster and more flexibly than previous [parallel](https://www.techtarget.com/whatis/definition/parallel) data transfer interfaces.

There are several components used in SCSI storage systems:

- **Initiator.** An initiator issues requests for service by the SCSI device and receives responses. Initiators come in a variety of forms and may be integrated into a server’s system board or exist within a [host bus adapter](https://www.techtarget.com/searchstorage/definition/host-bus-adapter). [ISCSI](https://www.techtarget.com/searchstorage/definition/iSCSI) connectivity typically uses a software-based initiator.
- **Target.** A SCSI target is typically a physical storage device (although software-based SCSI targets also exist). The target can be a hard disk or an entire storage [array](https://www.techtarget.com/searchstorage/definition/array). It is also possible for non-storage hardware to function as a SCSI target. Although rare today, it was once common for optical scanners to be attached to computers through the SCSI bus and to act as SCSI targets.
- **Service delivery subsystem.** The mechanism that allows communication to occur between the initiator and the target; it usually takes the form of cabling.
- **Expander.** Only used with serial-attached SCSI ([SAS](https://www.techtarget.com/searchstorage/definition/serial-attached-SCSI)); allows multiple SAS devices to share a single initiator port.


