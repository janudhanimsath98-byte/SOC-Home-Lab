# Lab 2 evidence log

Fill this in after running the lab in Packet Tracer. Do not mark a test successful until you have observed the result.

## Test matrix

| ID | Source | Destination | Expected result | Actual result | Evidence / notes |
|---|---|---|---|---|---|
| T1 | Staff PC 192.168.10.11 | Staff PC 192.168.10.12 | Pass (same VLAN) | Not run | |
| T2 | Finance PC 192.168.20.11 | Finance PC 192.168.20.12 | Pass (same VLAN) | Not run | |
| T3 | Staff PC | 192.168.10.1 | Pass (Staff gateway) | Not run | |
| T4 | Finance PC | 192.168.20.1 | Pass (Finance gateway) | Not run | |
| T5 | Staff PC | Finance PC 192.168.20.11 | Block (ACL) | Not run | |
| T6 | Staff PC | Service 192.168.30.10 HTTP/HTTPS (if configured) | Pass | Not run | |
| T7 | Admin PC 192.168.99.10 | SW1 192.168.99.2 via SSH | Pass (if SSH configured) | Not run | |
| T8 | Non-admin endpoint | Switch management SSH | Block | Not run | |
| T9 | Staff PC | Wrong-VLAN fault, then corrected | Fail during fault; pass after fix | Not run | |
| T10 | Endpoints across SW1–SW2 | Trunk fault, then corrected | Fail during fault; pass after fix | Not run | |

## Configuration evidence

- [ ] `show vlan brief` on both switches
- [ ] `show interfaces trunk` on both switches
- [ ] `show ip interface brief` on R1 and switch management interfaces
- [ ] `show ip route` on R1
- [ ] `show access-lists` on R1 after both permitted and denied tests
- [ ] Packet Tracer topology screenshot
- [ ] Sanitized final configurations

## Troubleshooting notes

### Fault 1 — endpoint placed in the wrong VLAN

- Intended VLAN and port:
- Symptom observed:
- Commands / checks used:
- Root cause:
- Fix applied:
- Retest result:

### Fault 2 — trunk is down or VLAN is not allowed

- Trunk endpoints:
- Symptom observed:
- Commands / checks used:
- Root cause:
- Fix applied:
- Retest result:

## Short report

### Design

Describe the VLANs, topology, address plan, trunk links, gateways, and ACL intent.

### Results

Summarize the tests that passed and failed. Link or refer to screenshots and saved configurations.

### Fixes and limitations

Record each fault and correction. Note any Packet Tracer device or command limitations and anything unresolved.
