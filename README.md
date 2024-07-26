Project in Early Development

# Net-BASH
Net-BASH is a decentralized communication tool that leverages the simplicity and ubiquity of bash scripting to create a resilient, user-controlled address and communications network. By harnessing fundamental networking protocols, Net-BASH bypasses centralized servers and obfuscates your data through inherent network obscurity.

## Planned Features:

* Direct peer-to-peer messaging over multiple ports, turning the internet itself into your communication backbone.

* Manual beaconing system to discover and connect with other users, building a self-managed address book free from central authorities.

* Optional PGP integration empowers those seeking identity verification, while a zero-trust architecture respects the anonymity of those who want it.


### Implementation Details:

#### Net Bashing Comms:

* Leverages raw data transmission over multiple ports, starting from the highest available and scaling downward as needed for bandwidth.

* Each message fragment includes a single-byte header to indicate its originating port for reassembly on the receiver's end.

* No reliance on centralized servers or DNS.

#### Passive Beaconing:

* Users manually initiate network scans for other devices.

* Beacons are simple messages requesting IP addresses from listening devices.

* Responding devices can include additional info (name, region, etc.) in their response.

* Address books are locally stored in text/markdown files, managed by the user.

#### Optional PGP Integration:

* Users can optionally sign their address data with their PGP private key for identity verification.

* Verification relies entirely on existing PGP tools and user practices – no key management within the system itself.

* Addresses with PGP signatures can be stored in the standard PGP address book format for compatibility with existing tools.

## Core Principles:

* Zero Trust: No device is implicitly trusted. Identity verification is optional and does not guarantee access or message delivery.

* User Control: Users have full control over their data, key management (if used), and communication channels.

* Simplicity: The system prioritizes simple, robust techniques over complex solutions. Obscurity is achieved through leveraging existing network infrastructure and user-controlled behavior.

## Future Considerations:

* Development of a user-friendly interface (ncurses CLI & KDE Kpart GUI).

* Smartphone / GSM / SMS Implementation
