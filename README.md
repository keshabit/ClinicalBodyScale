\# ClinicalBodyScale for Home Assistant

ClinicalBodyScale is a vendor-independent body composition engine for Home Assistant.

Unlike manufacturer-specific integrations, ClinicalBodyScale accepts weight and bioelectrical impedance measurements from any compatible scale and calculates clinically meaningful body composition metrics using validated algorithms such as OpenScale, Xiaomi, Sanitas, and Science mode.

\## Features



\- Vendor-independent

\- Single-frequency and dual-frequency BIA support

\- Multiple calculation engines

&#x20; - OpenScale

&#x20; - Xiaomi

&#x20; - Science

&#x20; - Sanitas / Beurer

\- Manual user profile

&#x20; - Height

&#x20; - Birthday or Age

&#x20; - Gender

\- Automatic profile matching

\- Home Assistant Config Flow

\- HACS compatible



\## Calculated Metrics



ClinicalBodyScale can calculate:



\- Weight

\- BMI

\- Body Fat %

\- Fat Mass

\- Lean Body Mass (LBM)

\- Muscle Mass

\- Skeletal Muscle Mass

\- Bone Mass

\- Total Body Water (TBW)

\- Protein %

\- Basal Metabolic Rate (BMR)

\- Visceral Fat

\- Metabolic Age

\- Body Type

\- Body Score



Dual-frequency scales additionally provide:



\- ECW (Extracellular Water)

\- ICW (Intracellular Water)

\- ECW/TBW Ratio

\- BCM (Body Cell Mass)



\## Supported Scales



ClinicalBodyScale works with any Home Assistant entity providing:



\- Weight

\- Impedance



Examples include:



\- Xiaomi Mi Scale

\- Xiaomi S400

\- ESPHome scales

\- BLE scales

\- MQTT scales

\- Template sensors

\- Future integrations



\## Installation



\### HACS



1\. Open HACS.

2\. Add this repository as a Custom Repository.

3\. Install ClinicalBodyScale.

4\. Restart Home Assistant.

5\. Add the integration from \*\*Settings → Devices \& Services\*\*.



\### Manual Installation



Copy



custom\_components/clinicalbodyscale



to



config/custom\_components/



Restart Home Assistant.



\## Configuration



Provide:



\- Weight Sensor

\- Impedance Sensor

\- Height

\- Birthday or Age

\- Gender

\- Calculation Mode



\## Calculation Modes



\### OpenScale



Implements equations derived from the OpenScale project.



Recommended for users seeking clinically validated body composition estimates.



\### Xiaomi



Implements Xiaomi body composition equations.



\### Science



Uses WHO/Schofield based metabolic equations with improved impedance modelling.



\### Sanitas



Implements Sanitas / Beurer style calculations.



\## Requirements



Home Assistant 2025.1 or newer.



\## Disclaimer



ClinicalBodyScale is intended for wellness and fitness purposes only.



It is \*\*not\*\* a medical device and should not be used for diagnosis or treatment.



\## License



MIT License

