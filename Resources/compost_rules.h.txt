// compost_rules.h — Auto-generated
// Thresholds from compost_dataset_realistic.csv
// Rule-Based Accuracy: 1.0000
#pragma once

// Feature priority:
// 1. Moisture    — PRIMARY
// 2. Temperature — SECONDARY
// 3. Methane     — LEAST IMPORTANT (not used)

// Soil Moisture ADC (resistance probe: HIGH ADC = DRY, LOW ADC = WET)
#define MOISTURE_WET_MAX  1500      // <= TOO_WET
#define MOISTURE_DRY_MIN  2000      // >= TOO_DRY

// DS18B20 Temperature (middle zone disambiguation)
#define TEMP_THRESH       29.09f   // > TOO_DRY

// 0 = COMPOST_READY | 1 = TOO_DRY | 2 = TOO_WET
