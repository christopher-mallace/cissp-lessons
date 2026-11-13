# DestCert CISSP — Domain 4 Course Video Material (Communication and Network Security)

Source: DestCert CISSP MasterClass course videos at https://new.my.destcert.com/schedule (Domain 4, main lesson videos only; MindMaps excluded — same scope as Domains 1–3).
Method: videos reviewed individually in small batches; each entry carries the lesson metadata (duration, URL, chapters, transcript block/phrase-line counts, reload-stability result) plus a detailed content summary of the instructor's teaching. Pulled 2026-11-13.
Note: Domains 7–8 are excluded from this project at Christopher's direction.

Schedule note: the first item listed under Domain 4 is "OSI Model Cheat Sheet" — a download, not a video, with no Transcript tab; it is not counted in the 43 main lesson videos (same treatment as non-video items in earlier domains).

---

## Video 1 — Introduction to Networks & Protocols
- Duration: 03:41 schedule (player 03:40; header flipped between the two across loads — transcript/chapters identical on all loads)
- Lesson: https://new.my.destcert.com/schedule/lesson/8caf7dd3-5391-4c27-a723-b9638f206909
- Chapters: Introduction 00:00; What is a Network? 01:23; What is a Protocol? 03:00
- Transcript: 00:11–03:00; 6 blocks / 54 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Domain 4 framing: understand networking before securing it, because networks are valuable organisational assets. A network is at least two devices connected so they can communicate — generally, a group of devices sharing the same rules for communication. What needs protecting is not just the network but the services, assets, resources, data and access it provides. Communication follows the human pattern: send, receive, interpret, act. Key definition: a protocol is a standard set of rules dictating how devices communicate — how they send and receive, interpret what arrives, and act on it.

---

## Video 2 — The OSI Model
- Duration: 17:26
- Lesson: https://new.my.destcert.com/schedule/lesson/9d3fed99-3a07-4c88-8d5e-ece43954f638
- Chapters: Introduction 00:00; What is the OSI Model? 01:34; Open System Interconnection (OSI) Model 02:11; OSI vs. TCP/IP 10:00
- Transcript: 00:13–16:53; 31 blocks / 264 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): OSI (Open Systems Interconnection) is a model, not an implementation — a layered architecture where each layer has its own responsibilities and none works alone. Layers top→bottom: 7 Application, 6 Presentation, 5 Session, 4 Transport, 3 Network, 2 Data Link, 1 Physical. Mnemonics: "All People Seem To Need Data Processing" (7→1) and "Please Do Not Throw Sausage Pizza Away" (1→7); knowing layer numbers is explicitly exam-relevant. Central trade-off: higher layers are more intelligent/functional and can make more security decisions but are slower with more overhead; lower layers are faster/more efficient but dumber — Layer 1 cannot make security decisions at all, while Layer 7 can do content filtering, deep packet inspection and antivirus. Security ideally applies at all layers, but the exam may ask for the best single layer for a purpose. Firewalls operate at Layers 3 (packet filtering — simple, fast decisions), 5 and 7 (application — more informed, less efficient). The instructor places SSL/TLS at Layer 4 (note: guide/other sources often place it differently — guide wording governs). He explicitly says the per-layer protocol/device slide does NOT need memorising — understand why each runs at its layer (functionality vs efficiency). TCP/IP is a protocol suite (an implementation of the OSI idea), named for TCP and IP; IP sits at Layer 3, TCP/UDP at Layer 4. Data flow: down the stack at the sender with each layer adding a header/trailer (encapsulation), up at the receiver (decapsulation). Data names by layer (PDUs): Layer 1 bits, Layer 2 frames, Layer 3 packets/datagrams, Layer 4 segments, Layers 5–7 data/information.

---

## Video 3 — Layer 1, Transmission Media & Crosstalk
- Duration: 06:26
- Lesson: https://new.my.destcert.com/schedule/lesson/f2d3a0ca-d5f8-477e-9c7f-b1698a699ad1
- Chapters: Introduction 00:00; Layer 1: Physical 01:01; Transmission Media 01:21; Crosstalk 05:34
- Transcript: 00:14–06:06; 10 blocks / 89 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): The OSI walk-through proceeds layer by layer (function, risks/security, devices/protocols per layer). Layer 1 connects devices, wired or wireless (wireless comes later). Wired media: twisted pair, coaxial, fiber optic. Exam framing flagged by the instructor: choose media by SECURITY advantage, not speed — do not pick fiber "because it's fast." Layer 1 is the least intelligent but fastest/most efficient layer; it only represents 0s and 1s (on twisted pair: +5 V = 1, −5 V = 0). Twisting the wire pair creates a magnetic field that contains the signal and resists crosstalk/noise/interference; shielded twisted pair adds further protection over unshielded. Coaxial (TV-cable style, centre copper conductor) has built-in shielding/integrity protection; its downside is cost and stiffness. Fiber optic is preferred today: best integrity, hardest to tap, most resistant to noise/interference/crosstalk. Crosstalk = one signal bleeding into another; the instructor's exam-style question — with which medium is crosstalk least an issue? — answer: fiber optic.

---

## Video 4 — Transport Architecture
- Duration: 07:05
- Lesson: https://new.my.destcert.com/schedule/lesson/ebddc50a-514a-4a8a-9b42-1b92e366e07f
- Chapters: Introduction 00:00; Transport Architecture 00:18; Topology 00:45; Data Plane 01:33; Cut-through & Store-and-forward 02:48; Control Plane 05:07; Management Plane 06:00
- Transcript: 00:18–06:46; 13 blocks / 99 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Transport architecture = how traffic moves through/across a network and how devices are arranged (topology). Three planes: the data/forwarding plane is the "doer" — it forwards traffic using a forwarding table and can only execute decisions it has been given; the control plane is the "brain" — it makes forwarding/routing decisions and builds the information the data plane uses; the management plane manages, configures and monitors the network and devices, including overseeing control-plane decisions. Central comparison: cut-through switching starts forwarding as soon as it has the destination header — faster, lower latency, but no error/integrity checking, so corrupt frames get forwarded; store-and-forward stores the whole frame, checks it, drops bad frames — slower but safer for integrity. The security lesson is that speed-vs-integrity trade-off.

---

## Video 5 — Network Topologies
- Duration: 18:46 schedule (18:45 on the lesson page)
- Lesson: https://new.my.destcert.com/schedule/lesson/4ff27df6-a81c-4aa4-a662-435a6deba8d6
- Chapters: Introduction 00:00; Network Topologies 00:37; Bus 02:25; Tree 06:19; Star 07:15; Mesh 08:44; Ring 09:35; Token 10:30; Physical vs Logical 12:11; Planes 13:39; Data Plane 14:01; Control Plane 14:24; Management Plane 15:05; Cut-through vs Store-and-forward 16:09
- Transcript: 00:20–18:23; 36 blocks / 277 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Topology = how devices are arranged/connected, physically and logically; the exam value is each topology's trade-offs and single points of failure. Bus: one shared cable, all devices see every transmission but only the recipient accepts it; one transmitter at a time or collisions occur; terminators stop signal reflection; a break in the shared cable can down the whole network. Tree: hierarchical bus/star hybrid branching from a root — scalable, but root failure affects everything below it. Star: all devices connect to a central switch/hub — one device's cable failure affects only it, but central-device failure affects all; easy to add/remove devices; the common modern layout. Mesh: devices interconnect with many/all others; full mesh = multiple paths, redundancy, fault tolerance at high cabling cost; partial mesh connects only some pairs. Ring: closed loop, traffic passes device to device in one direction; a single failure can break the ring unless dual-ring/backup exists. Token: a circulating token grants the right to transmit — orderly, collision-free (Token Ring). Physical vs logical topology can differ (physically star, logically bus/ring). The lesson closes by repeating the three planes and the cut-through vs store-and-forward trade-off from video 4, with the instructor urging focus on that contrast.

---

## Video 6 — Transmission Methods
- Duration: 04:54
- Lesson: https://new.my.destcert.com/schedule/lesson/76d09e9f-e1eb-4f44-87e2-db64749e99f7
- Chapters: Introduction 00:00; Transmission Methods 00:40; Unicast, Multicast, Broadcast 00:55; Anycast 02:50
- Transcript: 00:18–04:34; 9 blocks / 63 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Transmission methods: unicast = one-to-one; multicast = one-to-many; broadcast = one-to-all; anycast = one-to-any — requests go to any one of several equivalent nodes, typically the nearest/best, for lower latency and efficiency (CDNs such as Netflix are the standard example); the instructor notes anycast is specifically named in the exam outline. Main exam lesson: "security" is context-dependent across the five properties (confidentiality, integrity, availability, authenticity, non-repudiation) — never assume a security question means confidentiality. Unicast is best for confidentiality (one recipient only), while broadcast can be best for availability (everyone gets the message); a "which is more secure" question cannot be answered without its context. Caption warning: one line at ~01:04 renders "one-to-all" as "multicast" — that is a caption error; one-to-all is broadcast, as the following lines make clear.

---

## Video 7 — Traffic Flows
- Duration: 09:45
- Lesson: https://new.my.destcert.com/schedule/lesson/abbb4295-2242-455a-85fb-ef1102f99e18
- Chapters: Introduction 00:00; North-South & East-West Traffic Patterns 00:49; North-South Traffic 05:49; East-West Traffic 06:04; Considerations N-S & E-W Traffic 06:17
- Transcript: 00:19–08:17; 19 blocks / 117 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Data-centre traffic directions, still in the exam outline per the instructor. North-south traffic crosses the data-centre boundary (in or out; northbound = leaving toward the internet/external, southbound = entering; ingress/egress are the same in/out idea). East-west traffic stays inside, between servers, applications, services and segments. Traditional perimeter model: east-west was trusted by default, while north-south got the strict enforcement (firewalls, IDS, remediation) at the edge. Zero trust blurs the distinction: nothing is trusted based on origin, everything is verified, and all traffic gets stricter policy — implemented via more granular controls, attribute-based access parameters, continuous real-time monitoring and real-time reaction.

---

## Video 8 — Dealing with Collisions
- Duration: 08:32
- Lesson: https://new.my.destcert.com/schedule/lesson/0200d2c1-481c-42b3-b81d-40040ff32c0b
- Chapters: Introduction 00:00; Dealing with Collisions 01:26; Polling and Token 01:36; Carrier Sense Multiple Access 03:30; CSMA/CA 05:32; CSMA/CD 06:58
- Transcript: 00:18–07:49; 17 blocks / 123 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): On a shared bus, simultaneous transmissions collide; three historical answers: polling (ARCNET-style — every device repeatedly asks every other whether it has data; wasteful, obsolete), token passing (IBM Token Ring — only the token holder may transmit; orderly but inefficient at scale, and a failed device can stall the token; largely gone), and CSMA, the modern universal method: sense the carrier, transmit only when the wire is idle, then await acknowledgement. Collisions can still happen when two devices sense idle simultaneously. The key exam contrast: CSMA/CA (Collision Avoidance) is wireless — all 802.11 variants (b/g/n/a/c/ax) — avoiding collisions by separating send/receive channels; CSMA/CD (Collision Detection) is wired LANs — collisions are expected, detected via the voltage spike when signals collide, and the data is resent. Wireless = CA, wired = CD.

---

## Video 9 — Physical Segmentation
- Duration: 03:27
- Lesson: https://new.my.destcert.com/schedule/lesson/62aab876-dc57-46a5-b76c-58a7c45c0c8f
- Chapters: Introduction 00:00; Physical Segmentation 00:46; In-band Management 00:52; Out-of-band Management 01:39; Air-gapped 02:29
- Transcript: 00:19–02:57; 7 blocks / 43 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Physical segmentation is presented as one of the best ways to secure a network; this lesson ranks the management arrangements for a segmented network from least to most secure. In-band management: management traffic rides the same network as services — anyone with network access may reach the management capability, so it is least secure. Out-of-band management: a separate network manages the main one, with no real connection between them, so unauthorised users cannot reach management (same concept as out-of-band key distribution in the crypto material). Air-gapped: no connection possible at all — no physical or logical path in, wired or wireless — the most secure arrangement. Ranking to remember: in-band < out-of-band < air-gapped.

---

## Video 10 — Performance Metrics
- Duration: 10:36
- Lesson: https://new.my.destcert.com/schedule/lesson/632a04fa-f60c-43f9-b8fe-e8a136172187
- Chapters: Introduction 00:00; Performance Metrics 00:33; Bandwidth 01:14; Throughput 01:43; Pipe Example 02:00; Signal-to-Noise Ratio 06:11; Latency 09:11; Jitter 09:47
- Transcript: 00:19–10:15; 25 blocks / 139 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Bandwidth vs throughput must not be confused. Bandwidth = theoretical maximum capacity of a segment/channel/medium in bits per second (kbps/Mbps/Gbps) — it is capacity, not the speed bits travel (pipe analogy: a wider pipe carries more volume per unit time, not faster flow). Throughput = data that actually, successfully gets through per second — normally below bandwidth, equal only in the ideal case (no congestion, errors/retransmissions, overhead or hardware limits). Signal-to-noise ratio (SNR) is flagged as a must-know, including how to calculate it: SNR = signal power ÷ noise power, in decibels 10·log₁₀(signal/noise) — signal 10× noise = 10 dB, 100× = 20 dB, 1,000× = 30 dB; higher SNR = cleaner, more reliable signal. Latency = delay from source to destination (typically ms). Jitter = variation in latency (irregular frame arrival, degrades VoIP) — the instructor explicitly flags jitter as NOT on the exam, covered only because it affects quality of service.

---

## Video 11 — Layer 1 Devices
- Duration: 01:37 schedule (player 01:36)
- Lesson: https://new.my.destcert.com/schedule/lesson/2e570390-d830-414b-97fe-34a6ec3684c0
- Chapters: Introduction 00:00; Layer 1 Devices (Hubs, Repeaters, Concentrators) 00:28
- Transcript: 00:19–01:16; 3 blocks / 14 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Layer 1 devices — hubs, repeaters, concentrators — work only with bits and are unintelligent: they simply repeat what they receive. A repeater regenerates/cleans and strengthens a signal so it travels farther. A hub is a multi-port repeater: signal in on one port goes out all other ports. A concentrator is the same class of central multi-port Layer 1 device. Exam point: these devices are very fast but make NO forwarding or security decisions — no addressing, filtering or access control; they just flood/regenerate bits.

---

## Video 12 — Layer 2, Physical Addressing, and Circuit vs. Packet Switching
- Duration: 12:02 schedule (player 12:01)
- Lesson: https://new.my.destcert.com/schedule/lesson/3e5c8d74-935d-4c58-bd83-95559a737db3
- Chapters: Introduction 00:00; Layer 2: Data Link 00:39; Physical Addressing 01:43; Circuit Switched Network 04:11; Transmission of digital data over analog connections 06:08; Packet Switched Network 08:37; Circuit vs. Packet Switching 10:18; Virtual Circuits (PVCs & SVCs) 10:43
- Transcript: 00:13–11:43; 18 blocks / 176 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Layer 2 (Data Link) is the translator between Layer 3 (packets/datagrams) and Layer 1 (bits): it formats datagrams into bits downward and bits back into datagrams upward. Physical addressing lives here: the MAC address, a function of the network card, kept globally unique by structure (vendor/manufacturer portion + device-unique portion); logical addressing belongs to Layer 3. Circuit-switched networks (the PSTN/POTS telephone network) establish a dedicated full-duplex circuit before communication — built for analog voice. Digital data over that analog network needed modems (modulation/demodulation), capped around 56 kbps because the network itself is analog; DSL/cable modems are faster because they use different networks — which is why dedicated data networks were built. Packet-switched networks (all data networks) establish no circuit: data is chunked into individually addressed packets that may take different paths, arrive out of order or not at all, and are reassembled at the receiver. Virtual circuits on packet networks: a PVC is permanent (e.g. linking two offices over a provider WAN); an SVC is set up on demand and torn down after (a VPN connection is the instructor's example). Note: the instructor's voice-band (4,000–6,000 Hz) and 56 kbps figures are hedged in the lesson ("I think") — treat as approximate, guide wording governs.

---

## Video 13 — Authentication Protocols and Layer 2 Devices & Protocols
- Duration: 12:27 schedule (player 12:26)
- Lesson: https://new.my.destcert.com/schedule/lesson/26d1de57-43f6-4a30-8041-0042d8613395
- Chapters: Introduction 00:00; Authentication Protocols 00:15; SLIP 00:41; PPP 01:09; PAP 02:32; CHAP 03:50; EAP 05:01; PEAP 05:40; Common Types of EAP 06:35; Layer 2 Devices 07:59; Layer 2 Protocols 09:38
- Transcript: 00:13–12:11; 17 blocks / 180 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Authentication protocols for point-to-point/dial-up/leased-line connections, in historical progression. SLIP (Serial Line Internet Protocol, 1980s): carries IP only; no error detection/control, no compression, no security — legacy. PPP superseded it: multi-protocol encapsulation, built-in authentication, link-quality monitoring, compression, error detection. PAP (RFC 1334): two-way handshake, username/password in PLAIN TEXT, no encryption, no forced password change — weakest, legacy only. CHAP (RFC 1994): three-way challenge–response with an MD5 hash; the password is never sent, challenges change, periodic re-authentication is possible. EAP (RFC 3748): not one method but an extensible framework that negotiates authentication methods. PEAP: EAP inside a TLS tunnel — encrypted channel, server certificate, mutual authentication in typical wireless use. Common EAP types listed: EAP-MD5 and Cisco LEAP are the older/weaker ones; EAP-TLS is certificate-based with mutual authentication; EAP-TTLS and PEAP are the tunnelled approaches; also EAP-FAST, EAP-POTP, EAP-PSK, EAP-SIM, EAP-GTC. Centralised AAA services noted: RADIUS, TACACS/TACACS+, Diameter (taught in depth in Domain 5). Layer 2 devices: NICs, bridges, hubs, switches, wireless access points — bridges/switches learn MAC addresses, forward/filter frames, segment the LAN and reduce collisions; switches are multi-port MAC-table devices and the basis for VLANs. Layer 2 protocols: Ethernet, Token Ring, FDDI, Frame Relay, ATM, ISDN, X.25, HDLC, PPP, SLIP, plus tunnelling protocols L2TP, PPTP, L2F; the LLC and MAC sublayers handle flow/error control and addressing. Exam contrasts stressed: SLIP vs PPP; PAP (plain text, two-way) vs CHAP (hash, three-way); EAP as framework vs single method; PEAP as tunnelled EAP.

---

## Video 14 — More detail on Authentication Protocols
- Duration: 07:20
- Lesson: https://new.my.destcert.com/schedule/lesson/db81802f-dad3-420d-8b8c-2fcda6f23782
- Chapters: Introduction 00:00; Authentication Protocols 01:16; PAP 01:25; CHAP 02:18; EAP 02:57; PEAP 03:32; Common types of EAP 04:09
- Transcript: 00:19–07:01; 13 blocks / 95 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): A second, chart-driven pass over the video 13 protocols — the instructor emphasises knowing the comparison chart itself. PAP: two-way, plain text, low security, no challenge–response, no encryption. CHAP: three-way MD5 challenge–response (challenger sends ID + random challenge; peer returns a hash of the shared secret); password never transmitted; periodic re-authentication and replay protection make it stronger than PAP. EAP: the extensible framework (RFC 3748) carrying many methods over PPP and wireless. PEAP: EAP inside a TLS tunnel with a server certificate and an inner method (e.g. EAP-MSCHAPv2); the common wireless choice. EAP-type contrasts: EAP-MD5 (one-way, MD5, static password); EAP-TLS (mutual authentication, client AND server certificates — presented as most secure); EAP-TTLS (tunnelled, server certificate + inner method); PEAP (tunnelled, common for wireless); EAP-LEAP (Cisco, older, vulnerable); EAP-FAST (Cisco, protected access credential for fast re-authentication); EAP-SIM/EAP-AKA variants. Know how PAP/CHAP/EAP/PEAP differ in handshake, encryption, mutual authentication and use case.

---

## Video 15 — Layer 3 & Logical Addressing
- Duration: 08:19 schedule (08:18 on reloads — display difference only)
- Lesson: https://new.my.destcert.com/schedule/lesson/1d81cc40-28b0-4ba0-a2ad-f42823898a5c
- Chapters: Introduction 00:00; Layer 3: Network 00:41; Internet Protocol (IP) 01:10; Explanation of Internet Protocol 02:27; Logical Addressing 04:15; LAN Technologies 06:29
- Transcript: 00:15–08:04; 12 blocks / 122 phrase lines (stable in content across four loads; no alternate version)
- Content summary (not a verbatim reproduction): Layer 3 (Network) is the "captain" of the OSI team; in practice it is TCP/IP's IP. IP's two core jobs: fragmentation (breaking a message into datagrams) and addressing/delivery. The Layer 3 unit is the datagram = header (source/destination addresses, fragmentation fields) + payload. Logical addressing: IPv4 addresses are 32 bits (four 8-bit groups, dotted decimal) → 2^32 ≈ 4.3 billion unique addresses, a known finite limit. NAT is introduced as the stopgap that stretched IPv4; IPv6 is the long-term answer at 128 bits, and per the instructor includes IPsec natively (authentication + encryption). The closing section covers the IEEE as the standards body that ratifies LAN standards (802.11 family as the example) — explicitly flagged: do NOT memorise the individual IEEE document numbers or the 802.11 variant list for the exam; what matters is the IEEE's standardising role.

---

## Video 16 — IPv4 vs IPv6 and Layer 3 Devices & Protocols
- Duration: 12:36 schedule (player 12:35)
- Lesson: https://new.my.destcert.com/schedule/lesson/7ac4cb0d-f73c-47aa-bc52-225ed545d3af
- Chapters: Introduction 00:00; IPv4 vs IPv6 00:38; Internet Protocol v4 Datagram 01:00; Internet Protocol v6 Datagram 04:23; IPv4 vs IPv6 Comparison 06:47; Layer 3 Protocols 07:54; Layer 3 Devices 11:15
- Transcript: 00:14–12:24; 18 blocks / 178 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): IPv4 (still dominant): 32-bit addresses, dotted decimal, four 8-bit octets 0–255 → 2^32 = 4,294,967,296 (~4.3 billion). IPv6: 128-bit addresses in hexadecimal, eight 16-bit groups → 2^128 ≈ 340 undecillion. Header comparison: IPv4 header 20–60 bytes with fields incl. Version, IHL, Type of Service, Total Length, Identification, Flags + Fragment Offset, TTL, Protocol, Header Checksum, source/destination (32-bit each), Options; IPv6 header is a fixed 40 bytes — Version, Traffic Class, Flow Label (20 bits), Payload Length, Next Header, Hop Limit, source/destination (128-bit each) — with NO header checksum and fragmentation/options moved to extension headers. Other contrasts: IPsec optional in IPv4 vs built-in/mandatory in IPv6 (instructor's framing); NAT needed for IPv4, not for IPv6. IPv4 and IPv6 are NOT backward-compatible — transition needs tunnelling or dual-stack. Layer 3 protocols: IP; ICMP (diagnostics — ping, traceroute); IGMP (multicast group membership); IPsec (encryption + authentication alongside IP); ARP (IP → MAC, bridges Layers 3/2); RARP (MAC → IP, for a host that doesn't know its own IP at boot). Layer 3 devices: routers (forward between networks), multilayer/Layer 3 switches (switching + some routing), gateways (connect differently-working networks). Caption slip flagged: in the devices section the transcript says the devices "operate at layer two" — a spoken/caption error in a Layer 3 section; do not learn it as stated.

---

## Video 17 — Private IPv4 addresses & Network Classes (subnetting)
- Duration: 05:36 schedule (player 05:35)
- Lesson: https://new.my.destcert.com/schedule/lesson/d654a135-52ea-4f60-a993-8f6332aa2422
- Chapters: Introduction 00:00; Private IPv4 addresses 00:51; Private address ranges 02:22; Network Classes (subnetting) 04:02
- Transcript: 00:15–05:29; 8 blocks / 74 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Private IPv4 addresses (RFC 1918) are not routable on the public internet; a private-only device needs NAT to reach/be reached from the internet. The three ranges to know — explicitly exam-flagged, with the instructor warning that questions test whether a given 172.x address falls inside or outside the private block: Class A 10.0.0.0–10.255.255.255; Class B 172.16.0.0–172.31.255.255; Class C 192.168.0.0–192.168.255.255. Notation: 32 bits shown as four dotted 8-bit groups purely for human readability. Classes by first octet: A = 8-bit network portion, B = 16, C = 24; a subnet mask marks the network/host split; subnetting = dividing a network into smaller subnetworks. Worked example: Class B with 16 host bits → 2^16 = 65,536 minus 2 (network + broadcast) = 65,534 usable hosts. Explicit flag: deep subnetting skill is NOT needed for the exam (a network-admin concern) — know what subnetting is and the class boundaries.

---

## Video 18 — Layer 4, TCP & UDP
- Duration: 04:57 schedule (player 04:56)
- Lesson: https://new.my.destcert.com/schedule/lesson/534adfd1-b009-4c0f-aa6f-067557c9c344
- Chapters: Introduction 00:00; Layer 4: Transport 00:16; TCP & UDP 01:37; TCP vs. UDP Headers 04:13
- Transcript: 00:16–04:44; 11 blocks / 70 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Layer 4 (Transport) moves information between communicating entities — taught via a truck-and-road analogy (the protocol is the truck; the connection is the road built first when reliability is wanted). TCP: reliable, ordered, connection-oriented, sequenced — connection established first (time + overhead), delivery confirmed, segments follow in order. UDP: unreliable best-effort, no connection, no guarantees — "send and pray" — fast. The trade-off is the lesson: TCP buys reliability with overhead/speed; UDP buys speed with reliability. Use cases: TCP where reliability matters; UDP where speed matters more — streaming audio/video and DNS are the given examples. The header explains it: TCP's header carries much more information (slower to process), UDP's is minimal (fast). Analogy caution: the "one truck at a time" line illustrates ordered delivery, not a literal TCP limit.

---

## Video 19 — TCP 3-Way Handshake, Ports, and Layer 4 Protocols
- Duration: 11:50
- Lesson: https://new.my.destcert.com/schedule/lesson/c236eaca-38a3-45a0-9ae5-86ac568bbf96
- Chapters: TCP 3-Way Handshake 00:55; Ports 08:01; Layer 4 Protocols 10:37
- Transcript: 00:12–11:37; 17 blocks / 175 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): The TCP three-way handshake: A sends SYN with a random sequence number (example 1000) — randomness matters, because a predictable number invites session hijacking; B replies SYN-ACK (acknowledges 1001, sends its own random SYN, example 2000); A acknowledges 2001. The +1 acknowledgement proves receipt/completeness: expecting 1001 and receiving 1003 means two packets are missing and must be resent; every packet is acknowledged thereafter. Teardown is likewise graceful (FIN / ACK in both directions). SYN flood: SYNs arrive faster than the host's connection queue can process, filling it until the host shuts down — called very prevalent; the instructor's stated defence is a Layer 7 proxy intelligent enough to absorb/ignore the bombardment. Ports: 16-bit field → 65,536 values (0–65,535); well-known 0–1023, registered ~1024–49,151 (given approximately), dynamic/private above that. Port 80 = HTTP given as the example. Explicit exam guidance: do NOT memorise port numbers; DO know services' exploits/vulnerabilities and hardening — disable unneeded ports/services, use more secure versions, patch to latest. SSL/TLS named as the other major Layer 4 security protocol (covered in its own video later).

---

## Video 20 — Common Ports
- Duration: 05:18
- Lesson: https://new.my.destcert.com/schedule/lesson/29d2435b-5867-446a-877f-de2b9f9f5977
- Chapters: Introduction 00:00; Services 00:28; Common Ports (File Transfer Protocol, Secure Shell, Telnet, Domain Name System, Hypertext Transfer P… [chapter label truncated on the site]) 01:10
- Transcript: 00:19–04:55; 12 blocks / 70 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Short hardening follow-on to video 19. Explicit guidance repeated: do NOT memorise the ~65,000 port numbers; DO remember the well-known ports of services known to have exploits. Only two numbers are actually stated in this lesson: HTTP 80 and FTP 21 (SSH/Telnet/DNS are named in the chapter title but no numbers are spoken). HTTP has no built-in security — secure it by tunnelling through SSL/TLS → HTTPS. Telnet is presented as the most dangerous service in many network engineers' view. Hardening logic: if a service isn't needed, turn it off / block it at the firewall; if it is needed, use a more secure version, tunnel it through something that supplies the missing security, run the latest patched version, and monitor it. Examples: FTP (21, no native security) → mandate SFTP; Telnet has no secure variant → tunnel it across SSH (authentication, encryption, multiplexing).

---

## Video 21 — Layers 5, 6 & 7
- Duration: 10:08
- Lesson: https://new.my.destcert.com/schedule/lesson/27acc398-b1a4-4362-be03-34e284b19511
- Chapters: Introduction 00:00; Layer 5: Session 00:18; Layer 5: Protocols 01:34; Layer 6: Presentation 02:42; Layer 7: Application 04:18; Layer 7: Protocols 04:46; Layer 7: Devices 09:11
- Transcript: 00:13–09:50; 12 blocks / 160 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): In TCP/IP the top three OSI layers are all handled by the application. Layer 5 (Session) establishes sessions, usually remote — the VPN example: credentials (user ID, password, possibly a token OTP) are supplied, and PAP/CHAP/EAP provide the authentication the session setup depends on; named protocols: NetBIOS, RPC. Layer 6 (Presentation) handles character conversion, graphics and compression/decompression (codecs); the security concern is codecs as a malware hotbed — no industry codec standards, proprietary utilities everywhere — so vet/test codec utilities (e.g. in a sandbox) for malware/backdoors. Layer 7 (Application) is the user interface into the model (e.g. Outlook for email); its applications are "services," and the security focus is hardening, repeated per service: HTTP → HTTPS (TLS/SSL tunnel); FTP (among the most vulnerable) → Secure FTP where needed, off where not; TFTP has no security at all — standard practice is off; DNS has little built-in security → DNSSEC is the industry's protection initiative; Telnet (most vulnerable) → tunnel across SSH; SMTP = mail; SNMP = remote device administration — use version 3 or later. Layer 7 devices: gateways, and application proxy firewalls — the most intelligent/informed decisions of any firewall type, paid for in efficiency (firewall architectures get their own later section).

---

## Video 22 — Convergence & VoIP
- Duration: 08:10
- Lesson: https://new.my.destcert.com/schedule/lesson/c46f82c1-addc-41fc-8a79-9bc14c0302ea
- Chapters: Introduction 00:00; IP Convergence 00:25; Converged Protocols 01:11; Voice 01:49; VoIP Protocols 03:46; VoIP Security Vulnerabilities 05:44
- Transcript: 00:13–07:52; 8 blocks / 117 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): IP convergence = the ordinary TCP/IP data network now carrying multimedia, audio, video and storage traffic too (converged protocol examples: Fibre Channel over Ethernet, iSCSI). The headline case is voice — more accurately IP telephony: voice is digitised and packetised onto the data network instead of travelling on a separate voice network; VoIP protocols exist to manage packets arriving via different routes/out of order in real-time conversation. Named protocols: SIP (signalling) and SRTP (adds authentication + encryption for secure voice). Standards warning: VoIP is vendor-heavy with few open standards, so a vendor choice can lock you into that vendor's (possibly insufficient) security capabilities. Native VoIP has NO built-in confidentiality, integrity or availability — it inherits the data network's insecurities; encryption buys confidentiality but adds latency (the mobile-call delay effect), and integrity is hard because caller impersonation/number spoofing is easy with software. Vishing = phishing over VoIP, typically with a spoofed familiar number — a risk every company with IP telephony carries.

---

## Video 23 — Network Attacks: Eavesdropping, Actively Scanning and SYN Scanning & Flooding
- Duration: 13:59
- Lesson: https://new.my.destcert.com/schedule/lesson/433ecc51-3c31-4d58-afdc-da8c2b8685a3
- Chapters: Introduction 00:00; Network Attacks 00:49; Network Attack Phases (Reconnaissance, Enumeration, Vulnerability Analysis, Exploitation) 01:00; Network Attacks 05:34; Passive Attacks vs. Active Attacks 05:40; Threat Agents 06:45; Passively Eavesdropping 07:40; Actively Scanning Ports 09:30; SYN Scanning 10:27; SYN Flooding 11:38
- Transcript: 00:18–13:37; 25 blocks / 205 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Attacks run as a chain of phases in order — reconnaissance, enumeration, vulnerability analysis, exploitation — like the kill chain: break any phase and the attack fails, so defence means making each phase difficult or impossible. Reconnaissance = initial target information (domain names, IP ranges); defence: don't publish it, don't be an attractive target. Enumeration = specific detail (ports, services, OS/technology versions); defences include hardening, running nothing unneeded, and policies against staff posting internal tech details on forums/social media. Explicitly exam-flagged: passive vs active attacks are distinguished by DETECTABILITY — passive attacks are impossible/very hard to detect, active attacks are easily detectable; if it's detectable, it's active. Eavesdropping is the passive exemplar (listening without changing anything — the instructor acknowledges the promiscuous-mode objection but says the exam treats simple listening as passive). Port scanning and SYN scanning are active (packets are sent/probing is detectable; a SYN scan's response reveals open ports/services and possibly a stateful firewall). SYN flooding is a DoS attack (queue fills, host shuts down) and therefore active; defence is a SYN proxy that absorbs/ignores the flood rather than letting the host handle SYNs alone.

---

## Video 24 — Network Attacks: DoS & DDoS, Spoofing & ARP Poisoning
- Duration: 18:11 schedule (player 18:10)
- Lesson: https://new.my.destcert.com/schedule/lesson/29a635cd-4aad-437e-a063-2c481abb5130
- Chapters: Introduction 00:00; IP Based Attacks 00:58; DoS & DDoS 06:38; Man-in-the-Middle 08:22; Spoofing 10:03; Network Exploit Tools 11:04; ARP Poisoning 13:49
- Transcript: 00:12–17:51; 27 blocks / 269 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): IP-based attacks sit at Layer 3 and target IP's two functions: fragmentation attacks (overlapping-fragment and teardrop — remember only that both are DoS; details explicitly not needed) and addressing attacks. DoS = any attack that brings down a system/architecture/application's ability to function. Spoofing = pretending to be something/someone else (IP, MAC, user ID, email, DNS) — also called masquerading. Two spoofing-based DoS attacks to remember: Smurf (IP spoofing + ICMP echo flood; most organisations blunt it by blocking inbound ICMP, which also neuters ping/traceroute recon) and Fraggle (same pattern with UDP instead — much harder to defend because UDP can't be blocked; it carries streaming, VoIP, DNS). DDoS is a category of DoS: many compromised hosts (zombies) attack one target simultaneously. Man-in-the-middle: an intermediary who intercepts and can alter or DoS the traffic; the instructor's exam shortcut is that internet-originated attacks can be treated as MitM since the internet sits between networks (his framing, not a textbook definition). DHCP warning: it hands a joining device a trusted IP automatically, so network security should authenticate BOTH the node (e.g. by MAC/IP) and the user (knowledge/ownership/characteristics factors) after assignment. ARP poisoning: ARP maps IP→MAC via per-device tables with no security checks, so an attacker can claim another device's identity and receive/alter its traffic — and the instructor generalises: anything table-driven (routers, DNS, switches) shares the same weakness.

---

## Video 25 — Wireless Architecture, Technologies, Authentication, Encryption & TKIP
- Duration: 14:52
- Lesson: https://new.my.destcert.com/schedule/lesson/cb24aa5c-9861-49bf-813c-3ecdb4ccbd58
- Chapters: Introduction 00:00; Wireless Communication 00:20; Wireless Network Architecture 01:12; Radio Frequency Management 04:01; Wireless Radio Spectrum 04:52; Wireless Technologies 06:45; 802.11 Security Solutions 07:17; Wireless LAN Security Mechanisms 10:22; Wireless Authentication 10:54; Wireless Encryption 11:44; Wireless Integrity Protection 12:14; TKIP 13:29
- Transcript: 00:12–14:38; 16 blocks / 211 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Wireless architectures: ad hoc (peer-to-peer, no access point, often temporary) vs infrastructure (clients via an access point into the wired LAN/WAN). One AP + its clients = a Basic Service Set; multiple APs sharing one SSID = an Extended Service Set, enabling roaming. RF management: overlapping neighbours must not share a channel. Spectrum: 2.4 GHz has 11 channels with 1, 6, 11 the non-overlapping set; 5 GHz has more channels, less crowding, shorter range. 802.11 generations (speeds in Mbps/Gbps — captions render them as MB/s and GB/s): a = 5 GHz/54, b = 2.4 GHz/11, g = 2.4 GHz/54, n = both bands/up to 600 Mbps, ac = 5 GHz/up to 1.3 Gbps, ax (Wi-Fi 6) = up to 9.6 Gbps. Security (explicitly the exam focus — WPA and WPA2 must be known): hiding the SSID and MAC filtering are weak non-security (MACs are spoofable). Authentication: open-system and shared-key, then 802.1X with EAP and a RADIUS server; pre-shared-key (personal) vs enterprise mode. Encryption lineage: WEP (legacy, flawed, RC4-based) → WPA (interim, TKIP) → WPA2 (AES with CCMP — the secure standard). Integrity: TKIP's per-packet key mixing and its Message Integrity Check ("Michael"); TKIP itself is no longer secure — WPA2 in enterprise mode is presented as the best method.

---

## Video 26 — Common tools
- Duration: 04:44
- Lesson: https://new.my.destcert.com/schedule/lesson/b2d61241-0c9e-4b24-bbc1-95e1f5562305
- Chapters: Introduction 00:00; Common tools 00:29; ipconfig 02:08; ping 02:21; tracert, traceroute, tracepath 02:36; whois 03:20; dig 03:23; More common tools 03:55
- Transcript: 00:15–04:24; 7 blocks / 66 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Framing: a CISSP is an attractive target — attackers probe public-facing services and map networks with the same ordinary diagnostic tools defenders use to find and close gaps. High-level purposes only (explicitly flagged: deep knowledge of each tool is NOT exam-important; know what each does and how attacker/defender use it): ipconfig/ifconfig shows a host's IP, mask, gateway, DNS servers; ping tests reachability and responsiveness; tracert/traceroute/tracepath map the hop-by-hop route; whois looks up domain registration/ownership and name servers; dig is the precise DNS query tool; plus netstat (connections/listening ports), nslookup (DNS lookups), nmap (network mapping, port/service scanning) and Wireshark (packet capture/inspection).

---

## Video 27 — Network Virtualization Technologies: VLAN & SDN
- Duration: 09:37
- Lesson: https://new.my.destcert.com/schedule/lesson/5e8b5e9d-67d2-4573-91b5-6de57f436dca
- Chapters: Introduction 00:00; Network Virtualization Technologies 00:14; Virtual Local Area Network (VLAN) 00:44; Software-Defined Networks (SDN) 03:59; Traditional Network 04:27; SDN vs. Traditional Network 05:31; Advantages of SDN 06:18
- Transcript: 00:14–09:23; 14 blocks / 175 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Network virtualization = abstraction of the physical network. VLANs give logical segmentation on shared hardware: systems on the same switch are split into VLANs (e.g. VLAN 1 / VLAN 2 for departments that must not talk), only same-VLAN systems communicate directly, VLANs span multiple switches, and inter-VLAN traffic must pass through a router where rules apply — the cheap alternative to buying separate physical switches (physical segmentation). SDN extends the idea to the whole network: entire virtual networks run on one physical network. Key mechanism (recapping videos 4–5): in a traditional network every switch/router holds both planes and is configured individually; SDN separates the control plane out and centralises it — one central controller tells all devices how to forward, while the data plane just moves packets. Advantages, tied to public cloud: on-demand self-service provisioning with no physical rewiring (AWS/Azure/Google), programmatic configuration, virtual firewalls/routers/switches, and overlapping IP segments (many tenants can each use 10.0.0.1 in their own virtual network). SDN is presented as a fundamental building block of cloud resource pooling.

---

## Video 28 — SDN architecture
- Duration: 03:42
- Lesson: https://new.my.destcert.com/schedule/lesson/690ee9a3-b172-49e0-9536-d931fe6aa08f
- Chapters: Introduction 00:00; SDN architecture 00:36; Control Plane 00:56; Data Plane 01:03; Application Plane 01:20; What is an API? 01:37; Components that make up a network 01:55; Northbound APIs vs. Southbound APIs 02:24
- Transcript: 00:00–03:34; 8 blocks / 55 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Short SDN recap/extension: centralised software plus intelligent applications control the network — the foundation under cloud. Three planes now: control plane (decision-maker), data plane (forwards the actual packets as directed), and the application plane (the intelligent layer controlling everything across the architecture — in cloud contexts also called the management plane). An API (application programming interface) is the standard that lets architecture components communicate and pass information. Explicitly flagged as appearing in exam questions: northbound vs southbound APIs, defined relative to the control plane in the middle — northbound connects the control plane UP to the application plane; southbound connects it DOWN to the lower-level components/devices.

---

## Video 29 — Third-party connectivity
- Duration: 03:19
- Lesson: https://new.my.destcert.com/schedule/lesson/295c43f4-c14a-4a7d-8f7b-e653b512d383
- Chapters: Introduction 00:00; Network Security 00:15; Third-party connectivity 00:33; Physical Security 01:02; Evolution of Network Security 01:33; Third-party connectivity summary 01:43
- Transcript: 00:00–02:57; 4 blocks / 46 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Core instruction: inventory every connection from your network to untrusted networks and know exactly what exists — not just the internet/customer-facing side, but vendor and consultant connections too. The physical-security analogy: one entrance/exit is easiest to monitor and control; modern networks instead have many third-party connections, so the response is to understand and maintain the inventory, and secure each connection with firewalls and intrusion detection, firewall rules matched to the services/traffic crossing, and policies dictating the rules. The point singled out as most important: real-time monitoring so the organisation can react fast through incident management. (Standards for securing third-party/cloud connections are mentioned but none is named.)

---

## Video 30 — Wide Area Networks (WAN)
- Duration: 05:55
- Lesson: https://new.my.destcert.com/schedule/lesson/0e8a580f-49cd-4be0-ab1d-b19cc70f3564
- Chapters: Introduction 00:00; Wide Area Networks (WAN) 00:29; Wide Area Network (WAN) Technology 02:11; X.25 02:24; Frame Relay 03:14; Asynchronous Transfer Mode 03:32; Multi-Protocol Label Switching 03:42
- Transcript: 00:13–05:36; 9 blocks / 83 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): WANs connect devices across cities/countries, usually via provider-leased services: dedicated leased lines (T1/T2/T3), satellite/microwave links (large footprints, heavy natural interference hurting quality/integrity), or — what most companies use — provider data packet carrier services. Evolution of the packet carrier services, each replacing the last: X.25 (the original; still considered best for error correction, but the overhead makes speeds very limited) → Frame Relay (weaker error correction, faster) → ATM (Asynchronous Transfer Mode) → MPLS (Multi-Protocol Label Switching; faster, QoS, plus built-in security). The point the instructor repeats to remember: MPLS uses forwarding tables and label switching so a customer's path across the provider network is exclusively theirs and unreachable by other customers. Counterpoint he stresses: providers claim encryption is therefore unnecessary, but companies still encrypt — because the provider itself can reach the path, and paying for a service doesn't mean trusting the provider with the content; authentication and encryption may still be required according to the traffic's value.

---

## Video 31 — Monitoring and Management
- Duration: 06:57
- Lesson: https://new.my.destcert.com/schedule/lesson/8ab72a48-3cb4-4f49-bdb0-d75adf294cc7
- Chapters: Introduction 00:00; Monitoring and Management definition 00:50; Network Observability 02:03; Traffic Flow/Shaping 02:38; Capacity Management 03:16; Fault Detection and Handling 03:50; Performance Monitoring, Security Monitoring, Configuration Management, Log Management, Alerting & Notification, Reporting & Analytics, etc. 04:32
- Transcript: 00:19–06:36; 11 blocks / 100 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Monitoring and management = continuously examining the network, its services and its traffic for performance, reachability, reliability and security — ongoing work owed to internal and external stakeholders. The exam-outline items, each briefly defined: network observability (insight into how the network functions and whether it can deliver what stakeholders need); traffic flow/shaping (controlling how traffic moves, enforcing policy including security policy, prioritising some traffic over other traffic); capacity management (monitor demand, plan resources for today and anticipate tomorrow); fault detection and handling (spot and correct faults in real time so quality/integrity/availability don't degrade — incident management at network level); performance monitoring (the video 10 metrics); security monitoring (the five properties at the required level); configuration management (changes through rigorous change management with security built in); log management (read and react to logs promptly); alerting & notification (a SOC-style team watching, analysing and responding in real time). Closing point, repeated: security must be built into the monitoring/management of anything of value — networks, services, third-party connections.

---

## Video 32 — Network Defense Intro & Network Segmentation / Partitioning
- Duration: 48:02
- Lesson: https://new.my.destcert.com/schedule/lesson/85eb0bcd-f826-44d6-8e61-4f64edfb44f9
- Chapters: Introduction 00:00; 4.2 Secure Network Components 00:26; Network Segmentation / Partitioning 00:59; Partitioning definition 02:03; Network Perimeter 02:58; Edge Networks 05:30; Edge Computing 07:35; Edge Networks 15:30; Ingress 15:44; Egress 16:25; Peering 17:45; Public Autonomous System Number 23:54; Edge Router for BGP 24:23; Logical Segmentation 25:20; Virtual Local Area Networks (VLANs) 28:26; Virtual Private Networks (VPNs) 29:16; Virtual Routing & Forwarding (VRF) 30:55; Virtual Domain 31:51; Micro-segmentation 32:43; Network Overlays / Encapsulation 33:47; Distributed Firewalls 34:27; Distributed Routers 35:21; IDS/IPS 35:53; Zero Trust 37:02; Network Segmentation 38:38; Boundary Router 41:44; DeMilitarized Zone (DMZ) 42:48; Bastion Host 45:52
- Transcript: 00:18–48:00; 75 blocks / 690 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): The long core lesson for outline section 4.2 (Secure Network Components). Segmentation/partitioning divides a network into smaller subnetworks/zones (via routers, switches, firewalls, or logically) so each part gets proportionate policies — the purpose is containment: smaller attack surface, blocked lateral movement, protection of sensitive parts. The perimeter is the boundary between the trusted internal network and the untrusted outside (above all the internet); edge networks sit at that boundary. Edge computing processes data near where it is generated instead of hauling it to a central data centre/cloud — lower latency, less data moved. Ingress (in) and egress (out) both need controlling/filtering/monitoring — data leaving can itself be a security problem. Peering: two autonomous systems exchange traffic directly instead of via a transit provider (better performance/cost). An AS is a network/collection under one administration with a unified routing policy; a public ASN uniquely identifies it for inter-domain routing; BGP is the protocol edge/border routers use to exchange routing information between ASs. Logical segmentation techniques, each defined: VLANs (logical grouping, separate broadcast domains on shared switches); VPNs (encrypted tunnel over a public network — remote access or site-to-site); VRF (one physical router, multiple separate routing tables for tenants/traffic classes); virtual domains (logically separate domains on shared infrastructure); micro-segmentation (segmentation down to individual workloads/hosts/applications, restricting movement even inside a segment); network overlays/encapsulation (a virtual network built on the physical one); distributed firewalls (enforcement pushed to hosts/workloads, not just the perimeter); distributed routers; IDS (detect and alert) vs IPS (detect and block in line), deployable in distributed form. Zero Trust as the governing model: never trust by location, always verify identity/device/context, least privilege, assume breach. Perimeter components: the boundary router (edge first/last hop to the ISP, applies filtering); the DMZ (buffer subnetwork between internal network and internet hosting public-facing web/email/DNS servers — reachable from outside but isolated from the LAN, so a compromise doesn't yield internal access); the bastion host (a single heavily hardened, minimal-service host in the DMZ acting as the sole controlled entry/jump point, closely monitored because it is exposed).

---

## Video 33 — Proxy, NAT & PAT, and Private Addresses
- Duration: 07:48
- Lesson: https://new.my.destcert.com/schedule/lesson/0be34871-6cf8-4227-ad3f-60872e9c2a68
- Chapters: Introduction 00:00; Proxy 00:49; Proxy Server 01:06; NAT & PAT 03:08; Network Address Translation 03:42; Port Address Translation 04:50; NAT & PAT Example 05:36; Private Addresses 06:28
- Transcript: 00:13–07:29; 11 blocks / 118 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): A proxy acts on behalf of something else: requests are redirected to a purpose-built decider instead of clients connecting directly to servers. A proxy is a Layer 7 application, so it has the most intelligence for allow/deny decisions — the application proxy firewall is the exemplar (deep packet inspection, web content filtering). The user perceives a direct client–server connection; in reality the proxy sits in the middle enforcing the rules. NAT (presented as a Layer 7 function here) translates internal addresses to routable ones outbound and back inbound; its security value is hiding the internal addressing scheme — every attack starts with reconnaissance, so invisibility helps. PAT extends NAT: many internal machines share ONE external IP, distinguished by port numbers; the device tracks the mapping (source IP, destination IP, source port, destination port) so replies route back to the originating machine. Private addresses (RFC 1918) are non-routable, so NAT/PAT must translate them in both directions. Only the "10 dot" range is named aloud; the other ranges appear on the slide only. Flag tension: this instructor says the RFC 1918 ranges do NOT need memorising for the exam (only that they are private and non-routable) — but video 17 explicitly warned that questions test recognising whether a 172.x address falls inside 172.16–172.31. Learn the ranges (video 17 + guide) and treat this video's reassurance as the weaker source.

---

## Video 34 — Firewall Technologies
- Duration: 10:54
- Lesson: https://new.my.destcert.com/schedule/lesson/89d03aab-9fd3-4a7f-a861-2b2390f44727
- Chapters: Introduction 00:00; What is a Firewall 00:37; Firewall Technologies 02:07; Packet Filtering Technology 02:40; Stateful Packet Filtering Technology 03:48; Proxy Firewalls 05:34; Packet Filtering vs. Stateful Packet Filtering 08:17; Firewall Technologies (Summary) 09:30
- Transcript: 00:14–10:04; 16 blocks / 164 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): The distinction to keep straight: technologies = HOW a firewall decides; architectures (video 35) = HOW those technologies are deployed. A firewall allows/blocks traffic under predefined rules; it sits between two networks to protect them from each other, and inside a network between segments. It is a concept, not a device — as simple as a router deciding, or as sophisticated as applications doing deep inspection, content filtering, IDS and anti-malware. Recurring trade-off: higher OSI layer = more intelligence/functionality, less efficiency/speed. Only three technologies: (1) simple packet filtering — Layer 3, decides only on header fields (source/destination IP, packet type, service requested); simplest, fastest, most efficient. (2) Stateful packet filtering — also Layer 3, but keeps dynamic state tables (context/history of outgoing requests); a returning reply is allowed only if it matches the stored request (same machine, same protocol/request) — more informed, still Layer 3-limited. (3) Proxy firewalls — higher layers, most informed: circuit-level proxies at Layer 5 establish a session once correct credentials are supplied (user ID, password, possibly a 2FA number — VPN example); application-level proxies at Layer 7 are the most intelligent, programmable for any decision (content filtering, anti-malware, intrusion detection) because they read the data portion.

---

## Video 35 — Firewall Architectures
- Duration: 09:33
- Lesson: https://new.my.destcert.com/schedule/lesson/388af572-aae5-4a15-8594-21354de599b4
- Chapters: Introduction 00:00; Standard Firewall Architectures 00:31; Packet Filtering 01:54; Dual-Homed Host 03:00 (the panel shows only these 4 chapters; the screened-host, screened-subnet and N-legged material at 04:29–09:08 has no separate chapter buttons)
- Transcript: 00:13–09:08; 16 blocks / 137 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Architectures = how the video 34 technologies are put together/deployed. Explicitly exam-flagged: read the keywords and decide whether a question asks about TECHNOLOGIES or ARCHITECTURES. Four standard architectures in increasing security order: (1) Packet filtering — a Layer 3 router between internal network and internet; header-only decisions; very efficient, very limited. (2) Dual-homed host — a host/computer between the networks; a computer understands all 7 layers, so it can run any combination of the technologies (packet filtering, stateful, circuit-level or application-level proxy) — a better architecture. (3) Screened host — router outside facing the internet + the host in the middle; the router decides first and screens/protects the host (an attacker must compromise the router first), the host runs the richer technologies. (4) Screened subnet — adds an inside router too, so OUTGOING traffic is also monitored (data loss prevention; stopping internal machines being used as attack channels, e.g. DDoS). The inside/outside routers create sub-networks such as a DMZ: externally required services (web apps/servers for ordering and payment) live in the DMZ — protected and monitored — never on the internal network, which no untrusted entity may enter. Legs: the screened-subnet firewall is three-legged (internal / DMZ / internet), but there is no limit — four, five, a hundred legs, legs within legs: N-legged firewalls.

---

## Video 36 — IDS & IPS
- Duration: 04:39
- Lesson: https://new.my.destcert.com/schedule/lesson/a37a41f8-0612-4c35-a0c8-41898485f039
- Chapters: Introduction 00:00; Intrusion Detection & Prevention 00:30; Data Inspection 01:33; Applications of Data Inspection 01:55; Intrusion Detection System (IDS) 02:50; Intrusion Prevention System (IPS) 03:57
- Transcript: 00:14–04:33; 6 blocks / 66 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Framing principle: a complete control is preventive + detective + corrective. A firewall alone is only preventive, so detective/corrective capability must sit where firewalls sit — that capability is DATA INSPECTION: interpreting the packet's data portion (payload), not just the header, to recognise malicious intent, malware or attacks. Applications of data inspection: virus scanning, anti-malware, stateful inspection, web content filtering. The flagged contrast — understand the IDS/IPS difference: an IDS literally only detects; deployed in practice it triggers the corrective capability (e.g. signalling a firewall to drop packets/close connections), so the COMBINATION is preventive+detective+corrective. An IPS is the newer evolution: prevention, detection and correction all in line, in one technology.

---

## Video 37 — IDS & IPS: Host & Network Based
- Duration: 05:20
- Lesson: https://new.my.destcert.com/schedule/lesson/e35abd30-3491-41b2-9eb9-5fda19ea773a
- Chapters: Introduction 00:00; Types of IDS & IPS 00:48; Network Based IDS & IPS 01:02; Host Based IDS & IPS 01:11; Network based vs. Host based 01:25; IDS/IPS Network Architecture 01:56; Mirror / Span / Promiscuous Port 04:03
- Transcript: 00:03–05:10; 9 blocks / 77 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Recap: IDS vs IPS differ functionally, not in what they detect — an IPS is inline, so it prevents/detects/corrects at once; an IDS only detects and must be paired with preventive/corrective controls to form a complete control. The two deployment types (for both IDS and IPS): NETWORK-based — monitors traffic against rules via sensors placed strategically around the network; HOST-based — agents on important individual hosts (e.g. servers) watching host activity such as system-file changes and database access. Using both together gives strong detective coverage. Architecture follows the network: the DMZ needs detective capability too, and preventive/detective/corrective controls belong at every point, leg and connection. Monitoring is enabled by mirror/SPAN ports and promiscuous mode (a NIC accepting all traffic so it can be administered/monitored). Caution noted by the puller: the lesson's wording blurs switch port mirroring and NIC promiscuous mode — they are related but distinct mechanisms.

---

## Video 38 — IDS & IPS: Analysis Engines
- Duration: 07:44
- Lesson: https://new.my.destcert.com/schedule/lesson/b0a89af7-b07a-477d-a244-adcdbefbea18
- Chapters: Introduction 00:00; IDS/IPS Detection Methods 01:30; Ingress & Egress Monitoring 05:13; Whitelisting & Blacklisting 06:43
- Transcript: 00:13–07:16; 13 blocks / 107 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Network-based vs host-based are TYPES; this lesson covers the ANALYSIS ENGINES (the exam's term) that decide what is happening. Two engines: (1) Pattern matching / signature-based — recognises specific KNOWN attacks from vendor-supplied signatures; can only catch what it already knows, so signatures need regular updating (anti-malware analogy). (2) Anomaly-based — flags the unusual/abnormal, which first requires a learning period to establish what is normal (from stateful/historical data, statistics, usual protocols — e.g. a user who always uses TCP to the payroll database suddenly using UDP, or traffic reversing its usual direction). Its weakness is FALSE POSITIVES unless continuously fine-tuned; the fine-tuning theme (refining as false positives/negatives occur, improving over time) is flagged as exam-visible. Operational points: monitor BOTH ingress and egress — egress monitoring is growing in importance (DLP and more); and programme flagged items via whitelisting (allow from then on), blacklisting (never allow) and greylisting (defer the decision) — another learning mechanism.

---

## Video 39 — IDS & IPS: Detection Methods
- Duration: 06:09
- Lesson: https://new.my.destcert.com/schedule/lesson/be6a3a67-4230-4207-bf45-7437b9cd6689
- Chapters: Introduction 00:00; Sandbox 00:35; False Positives & False Negatives 01:21; Honeypots / Honeynets 03:21; Difference between Honeypots & Honeynets 04:11; Enticement & Entrapment 05:15
- Transcript: 00:13–05:53; 10 blocks / 90 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Focus: the CORRECTIVE actions after detection. Sandbox — a safe test environment where something suspect is run and judged (malicious or not, safe for production or not); an IDS/IPS can trigger sandboxing as its corrective action. False positives vs false negatives — explicitly flagged as exam material: a false positive reports an attack that isn't real (incident response launches, later stands down); a false negative is much more critical — a real incident the system should have caught is missed. Do NOT confuse these with biometrics Type 1/Type 2 and false reject/false accept terminology. Remedy: constant fine-tuning. ⚠️ Caption/speech slip flagged by the puller at ~03:03: the transcript says "raise the false negatives," which contradicts the lesson's own goal — the correct understanding is REDUCE false negatives; do not learn the phrase as stated. Honeypots/honeynets: fake, attractive environments that lure an intruder who has ALREADY entered away from the real systems (protecting them and potentially capturing evidence); the only difference is a honeynet is a COLLECTION of honeypots. Placement decides legality: ENTICEMENT (legal) lures someone who has already committed a crime/intruded; ENTRAPMENT (illegal) induces someone to commit a crime they were not contemplating. Place honeypots so the organisation entices, never entraps.

---

## Video 40 — Tunnelling & VPN
- Duration: 08:20
- Lesson: https://new.my.destcert.com/schedule/lesson/3d81b57a-954d-4564-aaec-be2456ab9e2a
- Chapters: Introduction 00:00; What is Remote Access? 00:53; Tunneling 01:35; Virtual Private Network (VPN) 04:25; Tunneling & VPN Protocols 05:27
- Transcript: 00:12–08:01; 11 blocks / 124 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Remote access = people travelling (hotel, coffee shop, home) connecting back into the internal network; secure remote access = a VPN. A VPN is built in two steps: TUNNELLING first — encapsulation, the whole original datagram (header + payload) placed inside the data portion of a second datagram whose new outer header dictates the path, forcing the packet along a specified route. Key correction: tunnelling alone gives NO security — the encapsulated data stays visible; security comes only from encrypting it. Formula: VPN = tunnelling + encryption; a tunnel without encryption is just a tunnel. Tunnelling protocols by layer (higher layer = more functionality/intelligence, less efficiency): Layer 2 — L2TP, L2F, PPTP; Layer 3 — IPsec (many experts' preferred approach; the network layer balances functionality/efficiency best for most organisations); Layer 4 — SSL/TLS; Layer 5 — SOCKS; Layer 7 — SSH. Flagged: all are tunnelling protocols that can typically provide encryption (hence VPN solutions), and the layers they operate at may be tested.

---

## Video 41 — GRE & split tunneling
- Duration: 05:43
- Lesson: https://new.my.destcert.com/schedule/lesson/2b344740-93f5-459f-a9d9-a945490d2232
- Chapters: Introduction 00:00; VPN 00:16; Tunneling 00:43; Generic Routing Encapsulation (GRE) 02:43; Split Tunneling 03:32
- Transcript: 00:16–05:31; 7 blocks / 79 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): Tunnelling without encryption is used for two purposes: (1) forcing traffic down a particular path (the new header specifies it), and (2) carrying packet types that could not otherwise cross the network — e.g. non-IP traffic (SCADA-related packets, IPX) across an IP network. GRE (Generic Routing Encapsulation) — named in the exam outline: a tunnelling protocol that does NOT support encryption, so it cannot technically be a VPN (a VPN requires tunnelling + encryption). Memorise: GRE only tunnels, never encrypts; its uses are exactly purposes (1) and (2). Split tunnelling — also named in the exam outline: normally a hotel traveller's internet traffic goes through the corporate VPN (encrypted, policy-controlled); with split tunnelling the user reaches the internet DIRECTLY via the local network while still connected to the company — saving bandwidth, but creating the dangerous state of simultaneous internal-network and untrusted-internet connections, bypassing corporate encryption and policy. Treat with caution.

---

## Video 42 — IPSec
- Duration: 06:48
- Lesson: https://new.my.destcert.com/schedule/lesson/18f8fd1c-66ec-409f-a432-c4b8ecfde8d0
- Chapters: Introduction 00:00; IPSec 00:24; Security Association (SA) 01:40; Internet Key Exchange (IKE) 02:31; IPSec Modes 03:22; IPSec Modes Diagrammatic Presentation 04:47
- Transcript: 00:13–06:20; 17 blocks / 117 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): IPsec — flagged as really important for the exam, expect many questions. One of the most-used VPN protocols; a Layer 3 (network layer) tunnelling protocol built into IPv6, used by routers. Security Association (SA): a one-way (SIMPLEX) tunnelling connection — two-way communication needs two SAs, one per direction; up to FOUR in total (both directions × separate authentication and encryption SAs). IPsec encrypts fast, so it uses symmetric cryptography — creating the key-distribution problem, solved by the Diffie-Hellman idea (both sides derive the same secret session key). Exam-critical distinction: IPsec's key-management protocol is NOT Diffie-Hellman itself but IKE (Internet Key Exchange) — a version of Diffie-Hellman doing the same job with different mathematics. Two sub-protocols: AH (Authentication Header) — integrity, data-origin authentication, replay protection; NO encryption. ESP (Encapsulating Security Payload) — everything AH provides PLUS encryption. Two modes: TRANSPORT (no tunnelling; original header reused) vs TUNNEL (datagram tunnelled, new header added). Four combinations: AH-transport, AH-tunnel, ESP-transport, ESP-tunnel — memorise the diagram; only ESP counts as a VPN, since a VPN is tunnelling + encryption.

---

## Video 43 — SSL / TLS & Remote Authentication
- Duration: 10:37
- Lesson: https://new.my.destcert.com/schedule/lesson/2b6a7bc6-b972-44a9-81f8-96a4d77261bc
- Chapters: Introduction 00:00; SSL / TLS 00:13; SSL / TLS Steps/Flow 03:46; Certificate Authentication 05:53; Symmetric Session Key and Encryption 07:08; Server Authentication 08:54; Does SSL/TLS Support Mutual Authentication? 09:09
- Transcript: 00:13–10:19; 11 blocks / 148 phrase lines (stable across three loads; no alternate version)
- Content summary (not a verbatim reproduction): SSL/TLS is the web's most-used security protocol (Amazon purchase, web banking). Two name traps stressed: SSL = Secure SOCKET Layer (not "Secure Session Layer"), and despite the name it operates at the TRANSPORT layer — the rename to TLS (Transport Layer Security) removed that confusion. TLS is simply the latest version of SSL (SSLv3 got minor improvements and was renamed rather than called SSLv4). The four-step flow (Amazon example; explicitly do NOT memorise the steps — understand how they work together): (1) Client Hello — the client signals it can communicate (browser/SSL version the server understands). (2) Server Hello + certificate — the server replies and sends its certificate, which contains the server's public key and is signed with the CA's private key. (3) Certificate validation = server authentication: the browser reads the issuer ID (VeriSign in the example), verifies the certificate with the CA's public key built into the browser (no warning pop-up = success); the server is thereby authenticated as genuine (spoofing would require the CA's private key) and the certificate's contents — above all the server's public key — can be trusted. (4) The client creates symmetric session keys, encrypts them with the server's public key, and sends them; only the server's private key can decrypt them, so both sides share the keys and all further traffic is symmetric-encrypted. Headline: SSL/TLS is a HYBRID — asymmetric cryptography exchanges the keys, symmetric cryptography does the bulk protection. Mutual authentication IS supported (the client sends its own certificate with the Client Hello and the server authenticates it), but it is not normally required on the web.
- CONFIRMED by this batch: video 43 is the LAST main lesson video in Domain 4; after it come only the Knowledge Assessment, assessment results, four MindMaps, Flashcards and Practice Questions.

---

# Appendix — Coverage mapping: Domain 4 videos → drill-list topics

All 43 main lesson videos are summarised above (metadata + content summaries; no verbatim transcripts in this domain). Mapping to the 38 Domain 4 topics in `DestCert-Need-To-Know-Drill-List.md`:

- 4.1.1 OSI Model → V2 (also V1)
- 4.1.2 Layer 1 Physical → V3
- 4.1.3 Transport Architecture → V4 (video-only in the guide; covered)
- 4.1.4 Network Topologies → V5
- 4.1.5 Transmission Methods → V6
- 4.1.6 Traffic Flows → V7
- 4.1.7 Dealing with Collisions → V8
- 4.1.8 Physical Segmentation → V9 (reinforced in V32)
- 4.1.9 Performance Metrics → V10
- 4.1.10 Layer 1 Devices → V11
- 4.1.11 Layer 2 Data Link → V12, V13
- 4.1.12 Authentication Protocols → V13, V14
- 4.1.13 Layer 3 Network → V15, V16
- 4.1.14 Logical Addressing → V16, V17 (private ranges/classes)
- 4.1.15 Layer 4 Transport → V18, V19, V20
- 4.1.16 Layer 5 Session → V21
- 4.1.17 Layer 6 Presentation → V21
- 4.1.18 Layer 7 Application → V21
- 4.1.19 Convergence & VoIP → V22
- 4.1.20 Network Security Attacks → V23, V24
- 4.1.21 Wireless → V25
- 4.1.22 Common Network Tools → V26 (video-only in the guide; covered)
- 4.1.23 VLAN & SDN → V27, V28
- 4.1.24 Third-party Connectivity → V29 (video-only in the guide; covered)
- 4.1.25 Wide Area Networks → V30
- 4.1.26 Monitoring and Management → V31
- 4.2.1 Network Segmentation → V32 (the 48-minute core 4.2 lesson; also V27)
- 4.2.2 Proxy, NAT & PAT → V33
- 4.2.3 Firewall Technologies → V34
- 4.2.4 Firewall Architectures → V35
- 4.2.5 Intrusion Detection and Prevention → V36, V37, V38
- 4.2.6 Sandbox → V39
- 4.2.7 Honeypots & Honeynets → V39
- 4.2.8 Endpoint Security → PARTIAL — no dedicated endpoint-security video among Domain 4's main lessons; V37's host-based IDS/IPS agents are the closest support
- 4.3.1 Tunneling & VPNs → V40, V41
- 4.3.2 IPSec → V42
- 4.3.3 SSL / TLS → V43
- 4.3.4 Remote Authentication → V43 (mutual authentication / client certificates; RADIUS/TACACS+/Diameter named in V13)

**Verdict: 37 of 38 Domain 4 drill topics fully covered by the main lesson videos; 4.2.8 (Endpoint Security) is partial.**

Stability: all 43 Domain 4 transcripts were STABLE across three loads each — no alternate versions anywhere in this domain. The only variations were 1-second schedule-vs-player duration-label differences on some videos and one panel-grouping quirk (V17). Cross-lesson tensions flagged in-file: V33 says the RFC 1918 ranges need not be memorised while V17 warns questions test recognising the 172.16–172.31 range (V17 + guide govern); V39's captions contain a "raise the false negatives" slip that contradicts the lesson's own goal (reduce them); V2 places SSL/TLS at Layer 4 while V40 lists it among Layer 4 tunnelling protocols and V43 confirms transport-layer operation, against V21's Layer 5–7 framing (guide wording governs).
