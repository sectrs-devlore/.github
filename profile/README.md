
<h1 align="center">Devlore: Device Interrupt Protection for Confidential VMs</h1>
<p align="center">
  <img src="https://github.com/user-attachments/assets/cb2bdd28-270b-4876-b878-25e2132e92b3" alt="Devlore logo" width="160">
</p>

<p align="center">
  Andrin Bertschi<sup>∗</sup>,
  Supraja Sridhara<sup>∗</sup>,
  Mark Kuhne, <br />
  Benedict Schlüter,
  Friederike Groschupp,
  Clément Thorens,
  Nicolas Dutly,
  Srdjan Capkun,
  and Shweta Shinde
</p>

<p align="center">
  ETH Zurich
  <br>
  <strong>RAID 2026</strong>
</p>

<!-- <p align="center">
  <a href="#">Paper</a> ·
  <a href="#">Code</a> ·
  <a href="#">Artifacts</a> ·
  <a href="#">BibTeX</a>
</p> -->

### Abstract

Modern confidential computing executes sensitive computation in an abstraction called confidential VMs and protects it from the hypervisor, host OS, and other co-resident VMs. It has been shown that an attacker can inject malicious interrupts to break the confidentiality and integrity of confidential VMs.

We present Devlore, a device interrupt isolation mechanism that protects confidential VMs from interrupt manipulation attacks. Our design employs a delegate-but-check strategy by offloading interrupt management to the hypervisor while adding correctness checks in trusted software.

We prototype our design on the Arm Confidential Computing Architecture (CCA). We evaluate it on Arm FVP using four diverse devices attached to confidential VMs and report costs on a Rock 5B board. Our case studies demonstrate the feasibility of real-world use cases, while Devlore incurs only 0.06% overhead for typical integrated GPU applications.
