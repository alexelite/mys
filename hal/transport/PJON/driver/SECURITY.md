## Security Policy
PJON is still in experimental phase and it distributed "AS IS" without any warranty, although a lot of work is iteratively done to make it more secure and reliable. Its implementation and specification are publicly available and are constantly reviewed worldwide by the community, the developers team and more recently by academics.

The security of a system that uses PJON for communication mostly depends on the vulnerabilities exposed by the hardware and by the physical layer used. Consider that **only air-gapped wired local buses are undoubtely secure**. When connecting a local bus to the internet using [ESPNOW](/src/strategies/ESPNOW), [EthernetTCP](/src/strategies/EthernetTCP) or [LocalUDP](/src/strategies/LocalUDP), [GlobalUDP](/src/strategies/GlobalUDP) or [DualUDP](/src/strategies/DualUDP), all connected devices must be considered potentially compromised. It should be considered a good practice not to connect to the internet systems that may cause damage (fire, flood, data-leak) if hacked.

### Safety warning
When installing or maintaining a PJON network, extreme care must be taken to avoid any danger. If devices are connected to AC power you are exposed to a high chance of being electrocuted if hardware is not installed carefully and properly. If you are not experienced enough ask the support of a skilled technician and consider that many countries prohibit uncertified installations. When a [SoftwareBitBang](/src/strategies/SoftwareBitBang) bus is installed [interference mitigation](https://github.com/gioblu/PJON/wiki/Mitigate-interference) and [protective circuitry](https://github.com/gioblu/PJON/wiki/Protective-circuitry) guidelines must be followed. When working with an [AnalogSampling](/src/strategies/AnalogSampling) LED or laser based setup safety glasses must be worn and transceivers must be operated cautiously to avoid potential eye injuries. Before any practical test or a hardware purchase for a wireless [OverSampling](/src/strategies/OverSampling), [ThroughSerial](/src/strategies/ThroughSerial) or [ThroughLoRa](/src/strategies/ThroughLoRa) radio setup, compliance with government requirements and regulations must be ensured.

### Reporting a Vulnerability
If you discover a vulnerability in the specification or in the implementation please report it as soon as possible opening an [issue](https://github.com/gioblu/PJON/issues). If you have developed a fix, feel free to open a [pull request](https://github.com/gioblu/PJON/pulls).