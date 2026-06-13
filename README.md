# My AZ-700 Lab Completion Log

## Lab: Unit 8 - Connect Two Azure Virtual Networks using Global Virtual Network Peering

**Date Completed:** [Today's Date]

**Status:** ✅ Complete

**Issues Encountered & Solutions:**

| Issue | Solution |
|-------|----------|
| Location 'East Europe' not available for VMs | Changed deployment location to West Europe |
| Standard_DS1_v2 SKU not available | Used Standard_D2s_v3 instead |
| Basic SKU public IP limit | Changed to Standard SKU with Static allocation |
| Peering only one direction | Created peerings in both directions |
| Ping fails after peering | Used RDP port test instead (Windows Firewall blocks ICMP) |

**Test Results:**
- Pre-peering: ❌ TcpTestSucceeded: False
- Post-peering: ✅ TcpTestSucceeded: True
