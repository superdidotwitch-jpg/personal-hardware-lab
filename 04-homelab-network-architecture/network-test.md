# Real network test — LAN gaming session

This was my first real-world validation of the homelab network. Rather than running synthetic benchmarks, I tested it the way I actually use it: a multiplayer gaming session with three devices running simultaneously.

## Scenario

A live multiplayer session with three devices active at the same time, using a mix of wired and wireless connections.

## Devices involved

| Device | Connection |
|--------|------------|
| Main gaming PC | Ethernet |
| Secondary PC | Ethernet |
| Nintendo Switch | Wi-Fi |

## Network path

Internet → ISP modem → TP-Link Archer MR500 router → unmanaged switch → both PCs via ethernet. The Nintendo Switch connected directly to the router over Wi-Fi.

## What I was testing

- Stability under multiple active users at the same time
- How the network handles mixed connection types (wired and wireless simultaneously)
- Real gaming performance — latency, disconnects, and general playability

## Results

All three devices connected successfully and the multiplayer session ran without major interruptions or failures. The network handled simultaneous traffic from all devices without issue.

## Observations

**Ethernet connections (main PC + secondary PC):**
- Stable and consistent throughout the session
- No drops or interruptions

**Wi-Fi (Nintendo Switch):**
- Stayed connected for the full session
- Performed adequately during gameplay — no major issues

**Unmanaged switch:**
- Distributed traffic between both wired devices without any visible bottlenecks

**Router (TP-Link Archer MR500):**
- Handled both wired and wireless clients simultaneously
- No crashes or signs of overload

## Limitations

This was not a rigorous test. I didn't collect measured data (no ping logs, no bandwidth metrics), it was a small sample of only three devices, and it was a short session rather than a long-duration stress test. Results reflect real usage but not controlled conditions.

## What this proves

My basic network topology works. The setup can handle multiple clients using mixed connection types at the same time. The infrastructure is functional — not just planned on paper.

## What comes next

- Add monitoring tools to measure latency and traffic properly
- Introduce dedicated network services (Raspberry Pi for Pi-hole/DNS, Mini PC for server/NAS)
- Explore network segmentation with VLANs down the line
- Run longer and larger tests as more devices are added
