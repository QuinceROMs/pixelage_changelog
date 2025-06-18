Project Pixelage device tree changelog
======================================

2025.06.18
----------
Signal quality and connectivity improvements:
- Reverted "Implement adaptive uplink power control" (due to significant energy consumption)
- Optimized RSRP and SINR thresholds for better signal quality
- Enabled advanced antenna diversity for Snapdragon X24 LTE modem
- Optimized carrier aggregation for energy-efficient performance
- Updated signal strength reporting for Android 15 compatibility.

Bluetooth enhancements:
- Implemented interference cancellation and channel estimation
- Deployed AI-driven adaptive frequency hopping for interference mitigation
- Optimized BLE connection intervals and scan parameters for stability
- Implemented improved adaptive RSSI filtering for signal quality enhancement
- Enabled advanced FEC (Forward Error Correction) and interleaving for robust data transmission
- Implemented spatial and polarization diversity for WCN3998 chipset.

Bluetooth power management:
- Enabled dynamic scheduler for WCN3998
- Reduced wakelock duration on ACL (Asynchronous Connection-Less) events
- Adjusted ELOG sleep parameters for WCN3998
- Enabled coex power-aware scheduling with Wi-Fi for better resource management
- Disabled unnecessary wakeup for inquiry scans to improve battery efficiency.

Audio quality enhancement:
- Added LDAC codec support for high-quality Bluetooth audio.

Added touch AIDL to device framework.

overlay: qssi: Removed deprecated config_mobile_tcp_buffers/networkAttributes.
