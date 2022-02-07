# Infrastructure as a Service
Using software deployed on wide range of commodity hardware, **Infrastructure as a Service** is the primary component of any true public cloud platform, it is the first level of abstraction of so-called bare metal hardware. Within these high level service categories, other specific sub-services are hiding, serving different use-cases. When composed together, a complete application can be deployed and managed throughout it's lifecycle, including seamless use by the end-users.

These services together create a service catalogue, from which a Solution Architect selects individual services, which are required to enable the given use-case higher up the service stack, or given application.

## Storage as a Service
Except for Random Access Memory (RAM) which we consider part of **Compute as a Service**, we count all other Data Storage types as an instance of **Storange as a Service**. We know Data Storage of several types, and with different characteristics suited for different use-cases:

- **Attachment Type** (*to consumer*)
  - Local (Host Attached) Storage
  - Local Area Network Attached Storage
  - Wide Area Network Attached Storage

- **Latency** (*how long it takes to access the stored data or confirm data writes*)
  - Time to first byte
  - I/O Operations per Second (*IOPS*)

- **Bandwidth** (*amount of data over a window of time a consumer can read or write* e.q. 100MB/s)
  - Ultra Low bandwidth (less than 10 Mb/s or 1.3 MB/s)
  - Low bandwidth (more than 10 Mb/s, but less than 50Mb/s)
  - Medium bandwidth (more than 50 Mb/s, but less than 250Mb/s)
  - High bandwidth (more than 250 Mb/s, but less than 10 Gb/s)
  - Ultra high bandwidth (more than 10 Gb/s)

- **Storage Capacity** (*amount of data a consumer can store for a given period of time*)
  - Low Capacity (less than 256GB)
  - Medium Capacity (more than 256GB less than 10TB)
  - High Capacity (more than 10TB less than 1PB)
  - Ultra High Capacity (more than 1PB)

- **Abstraction Type** (*how is the Data Storage type presented to the consumer*)  
    In practice, all data is effectively stored on **Block Storage**, but consumer may be provided with different abstractions, e.q. from File Storage to Object Storage to Block Storage; e.q. in case of *Cloud Shared Drive* such as **Google Drive**, or **Microsoft OneDrive**.
  - Block Storage
  - File Storage
  - Object Storage

- **Persistence Type** (*how long does the data persist*)
  - Volatile Storage (*does not persist after power-loss*)
  - Non-Volatile Storage (*persists after power-loss*)
    - Persistent Storage (*is intended as long-term location for given data, accessed regularly*)
    - Scratch Storage (*is intended as short-term location for given data, usually furing data processing*)
    - Archival Storage (*is intended as long-term location for given data, accessed sporadically*)
      - Write Once Read Many Storage (**WORM** - *most Blockchains are a type of Write Once Read Many replicated storage*)

## Compute as a Service 

## Network as a Service