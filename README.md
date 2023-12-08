# DFF-based PUF

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)


## Summary
The chip contains a DFFRAM array designed to evaluate the stability and reliability over various physical environment of DFF-based PUF using ML-assisted method to create initialization data.

It is designed to evaluate the GlobalFoundries process node for PUF design and help the development of the improved debiasing scheme. 

PUF-based key generation should further enhance the security of modern MCU and because the node is specifically targeting MCU, the PUF should use the same tech node.


## Why PUF Matters
When it comes to the confidentiality of MCU security, both firmware and sensitive information like keys and tokens should be protected.

The traditional method to secure such data is to use battery-backed solution so that the MCU could monitor the attacks actively. Lots of defense mechanisms require continuous power supply to function normally. Notably, the die shield route the cryptographically secure signal and any interruption would cause responses like destruction of the data enforced by the security policy.

However, the IoT application cannot afford such design because of its operating environment. So PUF Physical Unclonable Function (PUF) which is highly sensitive to external interference is the best alternative.