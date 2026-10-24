# Tänka sig! (Imagine That!)  
## Your own self-hosted, sovereign and hardened AI Box. Just like you would want it.
  
Tänka sig (taenkasig) is a proof-of-concept for deploying a private, hardened AI platform in your own on-prem environment.
Assuming you have capable metal, this repo will spin up a fully functioning AI/LLM server that runs on AlmaLinux OS.

The repo consists of provisioning playbooks written with Ansible (YAML) and Kickstart configs for the Anaconda installer.

## Design Philosophy

### Was AI used to write this?
Claude AI is used in **manual mode** throughout this project and every single line of code has been carefully vetted and questioned by a **human** before being accepted.  
Every design choice and every function in this repo has a justification for existing. So, while I'm only human, I can guarantee that where there was doubt research followed.

### What does it run on?

| Component      | Part                                                                                 |
|----------------|--------------------------------------------------------------------------------------|
| Case           | Zalman Z1 Iceberg White                                                              |
| Motherboard    | ASUS PRIME B550-PLUS                                                                 |
| Storage (OS)   | Kingston A400 SATA SSD (operating system and container images)                       |
| Storage (data) | Kingston NV3 2 TB M.2 NVMe SSD, PCIe Gen 4 (files are stored locally here)           |
| RAM            | 32 GB DDR4-3200 CL16: 2 × Kingston Fury Beast 16 GB kits (2 × 8 GB, KF432C16BBK2/16) |
| CPU            | AMD Ryzen 7 5700X                                                                    |
| CPU cooler     | MSI MAG CoreLiquid A13 240 Black                                                     |
| GPU            | Gigabyte GeForce RTX 5060 Ti WINDFORCE MAX OC 16 GB                                  |
| PSU            | Corsair RM750x, 750 W, ATX 3.1, 80 PLUS Gold                                         |


### Is it safe to use?
The intentions of this project are good but only you can assess your own risk appetite. This project aims to provide a simple way to deploy a **reasonably hardened and secure** AI/LLM Platform.  
Cyber security is never "turnkey". The security and threat landscape of AI/LLMs - Not to mention *tech in general* -  is **constantly changing**. You must assess your own risks and take reasonable precautions.  
