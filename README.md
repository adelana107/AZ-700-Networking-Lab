# AZ-700 Lab: Virtual Network Peering

## Lab Completed: 13-06-2026

### Resources Created

| Resource | Name | Details |
|----------|------|---------|
| Resource Group | ContosoResourceGroup | West Europe |
| Virtual Network 1 | CoreServicesVnet | 10.20.0.0/16 |
| Virtual Network 2 | ManufacturingVnet | 10.30.0.0/16 |
| VM 1 | TestVM1 | 10.20.20.4 |
| VM 2 | ManufacturingVM | 10.30.1.4 |

### Peering Configuration

| Peering Name | Status |
|--------------|--------|
| CoreServicesVnet-to-ManufacturingVnet | Connected |
| ManufacturingVnet-to-CoreServicesVnet | Connected |

### Test Results

| Test | Result |
|------|--------|
| Pre-peering connectivity | ❌ Failed (expected) |
| Post-peering connectivity | ✅ Succeeded |

### Key Takeaways

- Virtual network peering connects VNets through Microsoft backbone
- Peering must be bidirectional
- After peering, resources can communicate across VNets
- ICMP (ping) may be blocked by Windows Firewall but TCP/RDP works
