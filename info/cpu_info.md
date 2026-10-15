# SoC Compatibility & Performance Tiers

## Overview
LiveLens uses a tiered performance system to ensure stability across various Android hardware. Devices are categorized into tiers based on their System-on-Chip (SoC) capabilities, which dictates resolution limits, frame rates, and source counts.

---

## 🤖 Discord Bot Reference
If a user provides a phone model without specifying the CPU/SoC, the bot should prompt for the exact processor:
> **"Please provide your phone's CPU/SoC model (e.g., Snapdragon 8 Gen 2, Dimensity 9300) to determine compatibility."**

---

## 📊 Performance Tiers Detail

### 1. Entry Tier
**Compatible SoCs:** Snapdragon (460, 480, 480+, 4s Gen 2, 4 Gen 1, 4 Gen 2, 680, 662), Dimensity (6020, 6100, 700), Unisoc (T606, T610, T612, T616, T620, T700), Helio (P35, G35, G37, G80, G85, G88, G91), Exynos (850).

#### Resolution & FPS Limits
| Resolution | Standalone Max | With Game |
| :--- | :---: | :---: |
| **480p** | 30fps / 60fps | 30fps / 60fps |
| **720p** | 30fps | 30fps |
| **1080p** | ❌ | ❌ |
| **1440p** | ❌ | ❌ |
| **4K** | ❌ | ❌ |

#### Source Limits
- **Text:** 3 | **Image:** 2 | **Video:** 0
- **Web:** 1 | **GIF:** 1 | **VTuber:** 1 | **Sound:** 1

---

### 2. Low-Mid Tier
**Compatible SoCs:** Snapdragon (690, 695, 6 Gen 1, 6 Gen 3, 6s Gen 3, 750G), Dimensity (700, 800, 810, 900, 920, 1080, 6300, 7025), Helio (G95, G96), Unisoc (T820), Exynos (1280, 1330, 1380).

#### Resolution & FPS Limits
| Resolution | Standalone Max | With Game |
| :--- | :---: | :---: |
| **480p** | 30fps / 60fps | 30fps / 60fps |
| **720p** | 30fps / 60fps | 30fps |
| **1080p** | 30fps | ❌ |
| **1440p** | ❌ | ❌ |
| **4K** | ❌ | ❌ |

#### Source Limits
- **Text:** 4 | **Image:** 2 | **Video:** 0
- **Web:** 1 | **GIF:** 1 | **VTuber:** 1 | **Sound:** 1

---

### 3. Mid Tier
**Compatible SoCs:** Snapdragon (720G, 730, 730G, 732G, 750G, 765G, 768G, 778G, 780G, 7 Gen 1, 7s Gen 2, 7s Gen 3, 7 Gen 3, 845, 855), Dimensity (1000, 1100, 1200, 1300, 7200, 7300, 7400 Ultra, 8050), Helio (G99), Unisoc (T830, T850), Exynos (1080, 1480), Google Tensor.

#### Resolution & FPS Limits
| Resolution | Standalone Max | With Game |
| :--- | :---: | :---: |
| **480p** | 30fps / 60fps | 30fps / 60fps |
| **720p** | 30fps / 60fps | 30fps / 60fps |
| **1080p** | 30fps | 30fps |
| **1440p** | ❌ | ❌ |
| **4K** | ❌ | ❌ |

#### Source Limits
- **Text:** 5 | **Image:** 3 | **Video:** 1
- **Web:** 2 | **GIF:** 2 | **VTuber:** 1 | **Sound:** 1

---

### 4. Upper-Mid Tier
**Compatible SoCs:** Snapdragon (7+ Gen 2, 7+ Gen 3, 7+ Gen 4, 7 Gen 4, 782G, 855+, 870, 8s Gen 3), Dimensity (8000, 8100, 8200, 8300, 8400, 8400 Ultra, 8450, 8550, 9000 Lite), Exynos (1580), Google Tensor (G2, G3).

#### Resolution & FPS Limits
| Resolution | Standalone Max | With Game |
| :--- | :---: | :---: |
| **480p** | 30fps / 60fps | 30fps / 60fps |
| **720p** | 30fps / 60fps | 30fps / 60fps |
| **1080p** | 30fps / 60fps | 30fps / 60fps |
| **1440p** | 30fps | 30fps |
| **4K** | ❌ | ❌ |

#### Source Limits
- **Text:** 6 | **Image:** 4 | **Video:** 1
- **Web:** 2 | **GIF:** 3 | **VTuber:** 1 | **Sound:** 1

---

### 5. Flagship Tier
**Compatible SoCs:** Snapdragon (865, 888, 888+, 8 Gen 1, 8+ Gen 1, 8 Gen 3, 8s Gen 4), Dimensity (8500, 9000, 9000+, 9200, 9200+, 9500), Exynos (2100, 2200, 2400, 2500), Google Tensor (G4, G5).

#### Resolution & FPS Limits
| Resolution | Standalone Max | With Game |
| :--- | :---: | :---: |
| **480p** | 30fps / 60fps | 30fps / 60fps |
| **720p** | 30fps / 60fps | 30fps / 60fps |
| **1080p** | 30fps / 60fps | 30fps / 60fps |
| **1440p** | 30fps / 60fps | 30fps |
| **4K** | ❌ | ❌ |

#### Source Limits
- **Text:** 8 | **Image:** 5 | **Video:** 2
- **Web:** 3 | **GIF:** 3 | **VTuber:** 1 | **Sound:** 2

---

### 6. Ultra Flagship Tier
**Compatible SoCs:** Snapdragon (8 Gen 2, 8 Elite, 8 Elite Gen 5, 8 Elite Gen 6, 8 Elite 2), Dimensity (9300, 9400, 9500, 9600), Exynos (2600), Google Tensor (G6), Xiaomi (Xring O1).

#### Resolution & FPS Limits
| Resolution | Standalone Max | With Game |
| :--- | :---: | :---: |
| **480p** | 30fps / 60fps | 30fps / 60fps |
| **720p** | 30fps / 60fps | 30fps / 60fps |
| **1080p** | 30fps / 60fps | 30fps / 60fps |
| **1440p** | 30fps / 60fps | 30fps / 60fps |
| **4K** | 30fps / 60fps | 30fps |

#### Source Limits
- **Text:** 10 | **Image:** 6 | **Video:** 3
- **Web:** 4 | **GIF:** 4 | **VTuber:** 1 | **Sound:** 2

---

## Related Documentation
- [Performance Tiers & Source Limits](./performance_limits.md)
- [Troubleshooting Performance](../troubleshooting.md)
