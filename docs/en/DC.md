# Leonardo Data Centers

## General architecture

The Cloud Services described in the appropriate categories are hosted within 6 Data Centers distributed across Italy, set up in a dual-Region configuration (3 DCs + 3 DCs), each redundant with a pair of high-reliability Availability Zones. The data centers are equipped with all the necessary plant and technological infrastructure to ensure the highest quality standards in terms of reliability, availability, and physical security. 



The infrastructure configuration is fully redundant thanks to the division of each of the two Regions (North and South, hundreds of kilometers apart) into dual-AZs (Availability Zones), i.e., a pair of Data Centers in business continuity configuration, separated by several dozen kilometers as the crow flies.
Specifically, the two AZs are interconnected thanks to a proprietary backbone that guarantees complete redundancy, negligible latency, and private connectivity, logically characterizing the pair as a single virtual Data Center (Software Defined Data Center).  
The Regions are also interconnected via the same proprietary backbone and a network layer that enables a flexible, software-defined logical network architecture, ensuring the mobility of application loads and the inherent high reliability of Cloud solutions.  
Within an Availability Zone, workloads are distributed transparently, and the HA (High Availability) configuration enables infrastructure service continuity (Business Continuity) between the two data centers in the same Region.  
In fact, thanks to this basic configuration, the Cloud platform will also provide data distribution across the two zones of each Region. This configuration is possible thanks to the distribution of storage space (identified with the best Storage Array technologies available on the IT market) within the two AZs and, therefore, thanks to the continuous data replication of the service chosen by each individual organization. Thus, if an individual organization decides to leverage the full redundancy of its infrastructure (whether physical or virtual), it can leverage the Cloud platform's HA configuration and build DR/BC solutions.  
The Cloud platform's unique nature, thanks to the proprietary backbone interconnecting the two AZs constituting each Region, will enable synchronous and asynchronous data replication between the Storage Array systems constituting the Storage Layer. In this operational context, the individual organization will benefit from the Cloud platform's intrinsic ability to reactivate workloads within one of the two AZs or in a different Region. The restart of workloads protected by the activated DR/BC solution will then allow the individual organization to independently manage the restart of each application, according to its own DR or BC plans.

## Network description

The network is structured around three main components: Data Center Interconnection, Wide Area Network, and Local Area Network.

### Data Center Interconnection (DCI)

Interconnection between Data Centers relies on a high-capacity transport infrastructure built to ensure minimal latency, fault tolerance, and uninterrupted service.  
Key elements include:  

- IP/MPLS backbone, fully redundant and optimized for reliable, resilient routing.
- DWDM (Dense Wavelength Division Multiplexing) technology supporting high-capacity optical transmission with very low latency.
- VLAN-based segmentation, ensuring logical isolation of traffic domains and multi-tenant environments for different Public Administrations.
- Traffic management policies to regulate routing, priorities, and bandwidth allocation.  

The DCI enables the PSN to operate in a multi-region, dual–Availability Zone configuration—essential for high availability, synchronous/asynchronous replication, and business continuity.

### Wide Area Network (WAN) 

The WAN provides secure, high-performance connectivity to external networks, supporting access to PSN services as well as migration and integration activities for Public Administrations.  
It includes:
- Shared Internet/Infranet connectivity, offering controlled access to PSN services.
- Traffic profiling tools for bandwidth management, flow optimization, and congestion prevention.
- IDS and APM systems, ensuring threat detection and performance monitoring.
- Additional services, such as: 
    - Dedicated line aggregation.
    - VPN connectivity.
    - Special-purpose links for data migration.
    - Hosting of termination routers directly within PSN facilities.

The WAN ensures each Public Administration has isolated, secure channels for interacting with the infrastructure while maintaining high security and reliability.

### Local Area Network (LAN) 

The LAN infrastructure within each Data Center adopts a modular, redundant design with two possible configurations:
- Shared network devices, used by multiple PAs and deployed on one or two DCs.
- Dedicated devices, also deployable in single- or dual-site mode.  

The LAN is designed to guarantee:
- High availability.
- Strong segmentation of customer environments.
- Horizontal scalability.

It forms the communication backbone between compute, storage, cloud platforms, and security services within the PSN environment.

## Data Center characteristics

### General requirements and site criteria

The architecture is designed to meet high standards for security, resilience, and sustainability, aligned with TIER III certifications and current regulatory requirements.  
Data Centers are selected and designed to reduce environmental and external risks:
- Located in seismic zones classified as zone ≥3.
- Sited away from coasts, major rivers, and heavily trafficked areas.
- Positioned near metropolitan zones while maintaining low risk.
- Equipped with independent power feeds, not derived from the same medium/high-voltage substation.

Compliance with key regulations is ensured, including:
- Legislative Decree 81/2008 on workplace safety.
- Cabling compliant with ISO/IEC 11801 standards.

### Physical, structural, and infrastructural Features

Each Data Center provides:
- 100–350 m² of initial data-room space, expandable up to 700 m².
- At least 100 racks at project start (T0).
- Minimum 1,150 kW of available IT power.

Scalability is modular and aligned to PA adoption trends.

Supporting spaces include:
- Climate-controlled storage ≥ 50 m²,
- A shared Test Area
- Smart-working rooms for technicians and specialists,
- Dedicated, monitored loading/unloading bays separate from pedestrian access.

Thw structural and architectural characteristics are:
- Raised floors with ≥ 800 kg/m² load capacity,
- Access corridors at least 1200×2100 mm,
- Rack formats of 42, 48, and 52 units,
- Structures optimized for safety, energy efficiency, and operational continuity.

The Data Centers guarenteed strong sustainability measures. They include:
- Evaporative free cooling (EPV).
- Lithium batteries instead of lead-acid.
- Photovoltaic systems reducing PUE.
- Dynamic UPS (D-UPS) without batteries.
- Geothermal heat dispersers increasing cooling efficiency.

Older, energy-intensive systems are progressively replaced with more efficient technologies.

The electrical system meets TIER III requirements:
- Dual power feeds (A/B) to every rack.
- 230V–32A interlocked industrial sockets per power branch.
- Per-line monitoring of energy consumption and electrical loads.

The operational continuity is guaranteed even during maintenance of an entire electrical branch.

The Heating, Ventilation and Air Conditioning (HVAC) system ensures:

- Full redundancy and maintenance without downtime.
- Continuous environmental control.
- Dedicated hydronic/air networks.
- Energy optimization supporting TIER III compliance.

The physical security includes:

- Fire detection and anti-flood systems.
- Evacuation audio systems.
- Intrusion detection and CCTV.
- Physical access control (badge, biometrics).
- BEMS-based supervision and monitoring.

The internal DC network is structured into:

- Primary provider ingress network.
- Secondary distribution layers.
- “Meet Me Rooms” for secure interconnection with external carriers and networks.