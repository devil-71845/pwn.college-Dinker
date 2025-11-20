# CHEMISTRY OF ELECTRONIC MATERIALS & SENSORS - COMPREHENSIVE SUMMARY

---

## PART I: SENSORS

---

## 1. INTRODUCTION TO SENSORS

### Definition

**A sensor** is a device that converts an input of physical quantity into a functionally related output, usually in the form of an electrical or optical signal that can be read or detected either by human users or by electronic instruments.

### Key Functions

Sensors and their associated interfaces are used to detect and measure different physical and chemical properties, including:
- Temperature
- pH
- Force
- Odor
- Pressure
- Presence of special chemicals
- Flow
- Position
- Light intensity

### Characteristics of Sensors

**Essential characteristics:**

1. **Solely sensitive** to the chemical or physical quantity to be measured
2. **Insensitive** to all other parameters likely to be encountered in its application
3. **Does not influence** the properties of the input chemical/physical quantities while in operation

**Sensitivity**: Indicates the degree of variation of the output relative to the change in the measured chemical or physical property

### Selection Criteria for Sensors

Sensors should be selected based on:
- Selectivity
- Sensitivity
- Accuracy
- Calibration range
- Resolution
- Cost-effectiveness
- Repeatability
- Prevailing environmental conditions

---

## 2. CLASSIFICATION OF SENSORS

### A. Physical Sensors

**Definition**: Devices that measure and respond to specific physical conditions or changes in the environment

**Characteristics:**
- Measure physical responses (temperature, pressure, magnetic field, force, absorbance, refractive index, conductivity, mass change)
- No chemical interface
- Convert physical inputs into measurable electrical signals
- Essential for automation, monitoring, and controlling physical processes

| Type | Examples |
|------|----------|
| **Temperature Sensors** | Thermocouples, thermistors |
| **Pressure Sensors** | Barometers, piezoelectric sensors |
| **Mechanical Sensors** | Strain gauges, accelerometers |
| **Optical Sensors** | Photodiodes, CCD sensors |
| **Magnetic Sensors** | Hall effect sensors, fluxgate sensors |

### B. Chemical Sensors

**Definition**: Detect and measure chemical quantities and convert them into electrical signals

**Key Feature**: Has a chemically selective layer that responds selectively to a special analyte

**Process**: Deals with chemical information obtained from:
- Chemical reaction of the analyte
- Physical property of the system being probed

**Output**: Transformed into signals like conductance change, light, voltage, current, or sound

**Types:**
- **Biosensors**: Combine biological recognition element (enzymes, antibodies, nucleic acids) with transducer
- **Gas Sensors**: Detect and measure concentrations of various gases

### C. Biological Sensors

**Definition**: Sensors that directly utilize biological materials or properties to detect specific analytes or parameters

**Note**: Not necessarily involving a transduction mechanism

**Examples:**
- Blood pressure sensors
- Pulse oximeters

**Key distinction:**
- All biosensors are biological sensors
- Not all biological sensors are biosensors
- Biosensors specifically combine biological recognition element with transducer

### D. Electrochemical Sensors

**Operating principle**: Measurement of electrical properties (current, voltage, resistance) that change in response to chemical reaction at sensor surface

**Examples:**
- pH sensors (measuring acidity/alkalinity)
- Redox sensors (detecting oxidation-reduction reactions)

### E. Radiation Sensors

**Purpose**: Detect and measure various forms of radiation

**Types of radiation:**

1. **Ionizing Radiation**: Enough energy to ionize atoms/molecules
   - Examples: Alpha particles, beta particles, gamma rays, X-rays

2. **Non-Ionizing Radiation**: Less energy, cannot ionize atoms
   - Examples: UV radiation, IR radiation, radiofrequency radiation

**Sensor examples:**
- Infrared sensors (heat and motion detection)
- Ultraviolet sensors (detecting UV light intensity)

---

## 3. CHEMICAL SENSORS - DETAILED

### Definitions (IUPAC 1991)

"A chemical sensor is a device that transforms chemical information, ranging from concentration of a specific sample component to total composition analysis, into an analytically useful signal"

**Wolfbeis (1990)**: "Chemical sensors are small-sized devices comprising a recognition element, a transduction element, and a signal processor capable of continuously and reversibly reporting a chemical concentration"

### Characteristics of Chemical Sensors

- Transform chemical quantities into electrical signals
- Respond rapidly
- Maintain activity over long time period
- Small size
- Cheap
- Specific (respond exclusively to one analyte) or selective (to group of analytes)

### Components of Chemical Sensors

**Two basic components connected in series:**

1. **Chemical molecular recognition system (Receptor)**:
   - Interacts with analyte molecules
   - Physical properties change upon interaction
   - Signal appended to transducer

2. **Physicochemical transducer**:
   - Converts physical property changes to electrical signal
   - Sometimes receptor and transducer are same physical object

**Additional elements:**
- Signal amplification units
- Signal conditioning units

### Mechanism

**In majority of chemical sensors:**
- Receptor interacts with analyte molecules
- Physical properties change
- Transducer gains electrical signal

**Examples:**

**Metallic oxide semiconductor gas sensors:**
- Receptor = transducer (same object)
- Change electrical conductivity in contact with gases
- Conductivity change = measurable electrical signal

**Mass sensitive sensors:**
- Receptor and transducer = different objects
- Piezoelectric quartz crystal = transducer
- Sensitive layer at crystal surface = receptor
- Absorbs gas molecules → mass change → frequency change in electrical oscillator

### Applications of Chemical Sensors

- Monitoring manufacturing processes
- Environmental sensing
- Health monitoring
- Air quality monitoring
- Water quality monitoring
- Soil monitoring

### Selectivity Challenge

**Major limitation**: Inability to obtain selective response to target analyte given:
- Millions of known molecular species
- Variations in environmental conditions
- Variations in analyte amount/concentration (factors of 10²³ or greater)

**Solutions:**
- Develop analyte-specific films, membranes, coatings
- Incorporate preliminary sample separation (chromatography, electrophoresis)
- Miniaturize and integrate platforms with separation and detection systems

---

## 4. BIOSENSORS

### Definition (IUPAC)

"Biosensors are chemical sensors in which the recognition system utilizes a biochemical mechanism"

**Complete definition**: Self-sufficient integrated device using biological recognition element in direct spatial contact with transduction element to deliver qualitative or semi-quantitative analytical information

### Primary Characteristics

- Stability
- Economical
- Sensitivity
- Reproducibility

### Components of Biosensor (Three Main Components)

**1. Biological Element (Bioreceptor)**:
- **Function**: Binds the target molecule
- **Requirements**: Highly specific, stable under storage conditions, immobilized
- **Examples**: Tissue, cell, organelle, nucleic acid, microorganisms, enzyme, receptor, antibody
- **Purpose**: Precisely interact with target chemical, recognize when target nearby
- **Foundation**: Capacity to interact selectively with target chemical

**2. Transducer**:
- **Function**: Measures physical changes from bioreceptor reaction
- **Process**: Transfers energy into measurable electrical output
- **Acts as**: Interference between biological and electrical domains

**3. Detector**:
- **Function**: Amplifies and analyzes signals from transducer
- **Process**: Converts data to concentration units
- **Output**: Transferred to display device or data storage device

### Principle of Biosensor

**Two fundamental principles:**
1. Signal transduction
2. Biological element recognition

**Process:**

1. Biological components (enzymes, antibodies, nucleic acids, hormones, organelles, cells) incorporated as sensor/detector
2. Targeted bio-receptor often specific deactivated analyte
3. Transducer situated close to inactive enzyme
4. Measured analyte interacts with specific enzyme bio-receptor
5. Change in enzyme's biochemical properties
6. Electroenzymatic method produces electrical response
7. Transducer output (electrical signal) = direct representation of biological substance

### Step 1: Biorecognition

**Common bioreceptor choices and mechanisms:**

**A. Enzymes**:
- Highly specific catalysts for biochemical reactions
- Example: Glucose oxidase in glucose biosensor
  - Binds to and oxidizes glucose
  - Consumes oxygen
  - Produces hydrogen peroxide and gluconic acid
  - Causes pH change

**B. Antibodies**:
- Used in immunosensors
- Specifically recognize and bind to antigens (target analyte)
- Binding event detected and measured
- Determines presence or concentration of antigen

**C. Nucleic Acids (DNA)**:
- Used in genosensors
- DNA probes detect specific gene sequences
- High selectivity of complementary base pairing
- Identifies target nucleic acid

**D. Whole cells or microorganisms**:
- Required when detection needs complex biological system
- Example: Microorganism with specific metabolic pathway detects particular pollutant

### Step 2: Transduction

**Types of transducers and their principles:**

**A. Electrochemical**:
- Based on changes in electrical properties:
  - Current (amperometric)
  - Voltage (potentiometric)
  - Impedance (impedimetric)
- Mechanism (Amperometric glucose biosensor):
  - Glucose oxidase + glucose → redox reaction
  - Generates current proportional to glucose concentration

**B. Optical**:
- Detect changes in light properties:
  - Absorption
  - Fluorescence
  - Surface plasmon resonance (SPR)
- Mechanism (SPR):
  - Analyte binds to bioreceptor on metallic surface
  - Alters refractive index
  - Changes angle of light reflection
  - Detected by photodetector

**C. Mass-based (Piezoelectric)**:
- Piezoelectric crystal's resonant frequency changes when mass added to surface
- Mechanism:
  - Analyte binds to bioreceptor on crystal
  - Mass increases
  - Change in crystal's vibrational frequency measured

**D. Thermal (Calorimetric)**:
- Based on heat produced/absorbed during biochemical reaction
- Mechanism:
  - Thermistor measures temperature difference
  - Before and after solution passes over immobilized enzyme column

### Step 3: Signal Processing and Display

**1. Signal Conditioning**:
- Raw electrical output amplified
- Filtered to remove noise
- Produces clearer signal

**2. Analog-to-Digital Conversion**:
- Analog electrical signal → digital signal
- Easily processed and stored by microprocessor

**3. Data Processing**:
- Microprocessor interprets digital data
- Translates into meaningful quantitative/qualitative results

### Applications of Biosensors

- Medical diagnostics
- Blood glucose monitoring
- Drug screening
- Food quality control
- Environmental monitoring
- Bioprocess monitoring

---

## 5. GAS SENSORS

### Definition

Devices that detect the presence of gases in the environment and convert this information into an electrical signal

### Applications

- Monitor air quality
- Detect toxic or flammable gases
- Ensure safety in various industries

### Illustrative Example: Hydrogen Gas Sensor

**Importance**: Detection crucial in:
- Environmental pollution detection
- Indication of certain diseases
- Early sign of fire
- Reactor safety in nuclear power plants

**Types of Hydrogen Gas Sensors:**

**a. Catalytic Bead Sensors**:
- **Principle**: Catalytic combustion
- **Components**: Platinum wire coil coated with catalyst (palladium or platinum)
- **Operation**: H₂ contacts catalytic bead → reacts with catalyst → oxidizes → releases heat → change in resistance of platinum coil → measured and converted to gas concentration

**b. Semiconductor Sensors**:
- **Principle**: Changes in conductivity
- **Material**: Semiconductor (typically tin dioxide, SnO₂)
- **Operation**: H₂ contacts semiconductor → change in conductivity → measured for gas concentration

**c. Metal Oxide Sensors**:
- **Principle**: Changes in resistance
- **Material**: Metal oxide film (SnO₂ or WO₃)
- **Operation**: H₂ contacts metal oxide film → change in resistance → measured for gas concentration

### Hydrogen Gas Sensors Using Catalytic Bead Sensors (Pellistor)

**Detection method**: Hydrogen burns on heated, catalytically active surface

**Process**: Exothermic reaction → increases temperature of active bead → alters electrical resistance → measured by Wheatstone bridge circuit → determines gas concentration

**Application**: Widely used in industrial settings for safety monitoring within Lower Explosive Limit (LEL) range

#### A. Setup and Components

**Two main beads housed in flame-proof, porous casing:**

1. **Active bead**:
   - Fine platinum wire coil embedded in ceramic (alumina) bead
   - Coated with catalyst (platinum or palladium)
   - Lowers ignition temperature of hydrogen

2. **Reference bead**:
   - Matching ceramic bead with embedded platinum coil
   - WITHOUT catalyst
   - Compensator bead (inert)
   - Negates external environmental effects (temperature, humidity, pressure)
   - Prevents false readings

3. **Wheatstone bridge circuit**:
   - Active and reference beads connected into this electrical circuit
   - Non-hazardous atmosphere → bridge balanced, output voltage = zero

#### B. Working Principle

**Step 1: Heating the beads**:
- Continuous electrical current through platinum coils
- Heats beads to operating temperature (500-550°C)
- Requires input voltage (Vin)

**Step 2: Hydrogen diffusion**:
- H₂ gas present → diffuses through porous sensor casing
- Reaches both beads
- Requires ≥10-12% oxygen in atmosphere

**Step 3: Catalytic combustion**:
- H₂ molecules contact heated, catalytically coated active bead surface
- **Reaction**: 2H₂ + O₂ → 2H₂O (exothermic, releases heat)
- Reference bead (no catalyst) → temperature unchanged

**Step 4: Resistance change**:
- Heat from combustion increases active bead temperature significantly
- Platinum wire has positive temperature coefficient of resistance
- Temperature rise → increase in electrical resistance of active bead's coil

**Step 5: Wheatstone bridge imbalance**:
- Change in active bead resistance unbalances bridge
- Reference bead resistance unchanged
- Circuit produces measurable output voltage (Vout)
- Vout proportional to resistance difference between beads

#### C. Calibration Process

**Routine calibration using zero and span gases:**

**1. Zero calibration**:
- Sensor exposed to zero air (0% target gas)
- Establishes baseline reading
- Wheatstone bridge balanced to produce zero output voltage

**2. Span calibration**:
- Sensor exposed to known H₂ concentration (e.g., 50% LEL)
- Measured output adjusted to correspond to this concentration
- Establishes sensor's linear response curve

#### D. Limitations of Catalytic Bead Sensors for Hydrogen

1. **Oxygen dependency**: Requires minimum 10% O₂ by volume; fails in oxygen-deficient environments
2. **Poisoning**: Catalyst permanently damaged by silicones, lead, sulfur compounds
3. **High power usage**: Constant bead heating requires significant power; unsuitable for low-power/battery devices
4. **Sensitivity range**: Ideal for LEL range (explosion prevention), less effective for ppm levels

### Applications of Gas Sensors

**i. Industrial Safety**:
- Oil and gas, chemical manufacturing, mining
- Detect toxic and explosive gases
- Prevent accidents

**ii. Environmental Monitoring**:
- Air quality monitoring stations
- Vehicle emissions testing
- Indoor air quality monitoring
- Detect pollutants

**iii. Healthcare**:
- Anesthesia machines
- Ventilators
- Oxygen concentrators
- Monitor gas concentrations
- Ensure patient safety

**iv. Fire Detection**:
- Detect smoke and combustion byproducts
- Activate alarms or suppression systems

---

## 6. ROLE OF CHEMICAL SENSORS IN ENVIRONMENTAL MONITORING AND MEDICAL DIAGNOSTICS

### Environmental Monitoring

**A. Air Quality Monitoring**:
- Detect pollutants: NO₂, SO₂, CO, particulate matter
- Example: Electrochemical sensors measure NO₂ levels (vehicle and industrial emissions)
- Assess air quality
- Determine effectiveness of pollution control measures

**B. Water Quality Monitoring**:
- Detect contaminants: Heavy metals, organic pollutants, microbial contaminants
- Example: Ion-selective electrodes detect lead and mercury in water
- Ensure safe drinking water
- Monitor health of aquatic ecosystems

**C. Soil Monitoring**:
- Measure pH, moisture content, nutrient levels
- Example: Nutrient sensors detect nitrogen, phosphorus, potassium
- Aid precision agriculture
- Prevent over-fertilization and environmental damage

### Medical Diagnostics

**A. Blood Glucose Monitoring**:
- Diabetic patients monitor blood sugar levels
- Real-time data
- Adjust diet/medication to maintain stable glucose

**B. Breath Analysis**:
- Analyze breath for compounds indicative of medical conditions
- Example: Breath sensors detect acetone (elevated in diabetes)
- Non-invasive glucose monitoring method

**C. Drug and Alcohol Testing**:
- Detect drugs or metabolites in saliva/breath
- Measure blood alcohol concentration
- Monitor consumption, enforce sobriety laws

---

## 7. ELECTROCHEMICAL SENSORS

### Definition

Devices that detect presence of specific gases or chemical compounds through electrochemical reactions

### Key Advantages

- High sensitivity
- Selectivity
- Low power consumption
- Immediately generate electric signals

### Classification Debate

**Some scientists exclude conductance probes** because:
- Based on physical properties of ions moving in solution interior
- Not based on running chemical reactions
- Far from where electrochemical processes occur

**Solution**: Include electrode interface in conductance measurements
- Define equivalent resistances for electrode interface processes
- Combine all partial resistances → complex resistance (impedance)
- Impedance includes contributions from bulk solution and electrode interface
- Terms "conductance sensor" and "impedimetric sensor" often synonymous

### Classification by Working Principles

| Sensor Type | Transducer Principle | Measured Quantity |
|-------------|---------------------|-------------------|
| **Potentiometric** | Energy conversion | Voltage (high impedance) |
| **Amperometric and Coulometric** | Limiting current | Current (low impedance) |
| **Conductometric and Impedimetric** | Resistive | Resistance (reciprocal of conductance) |

### Principle of Operation

**Three main components:**

1. **Sensing electrode**: Made of material sensitive to target gas
2. **Reference electrode**: Provides stable reference potential for accurate current measurement
3. **Electrolyte**: Medium for ion movement

**Process:**
- Target gas contacts sensing electrode
- Chemical reaction occurs
- Generation or consumption of ions in electrolyte
- Generates small electrical current
- Current magnitude proportional to gas concentration

### Types of Electrochemical Sensors

**a. Potentiometric Sensors**:
- Measure potential difference between reference and working electrode
- Applications: pH sensing, ion-selective measurements

**b. Amperometric Sensors**:
- Measure current from oxidation/reduction of analyte at working electrode
- Applications: Detecting gases, biomolecules, pollutants

**c. Conductometric Sensors**:
- Measure conductivity changes from analyte-sensor surface interaction
- Applications: Detecting gases, ions, volatile organic compounds

---

## 8. EXAMPLE: CONTINUOUS GLUCOSE MONITORING (CGM) SENSOR

### Overview

**Definition**: Blood glucose sensor (CGM) that automatically measures glucose levels throughout day and night by detecting glucose in interstitial fluid

**Data transmission**: To receiver, smartphone app, or insulin pump

### A. Components of a CGM Device

**Three main parts:**

**1. Sensor**:
- Small, disposable electrode filament inserted just under skin
- Tip coated with enzyme (typically glucose oxidase, GOx)
- Reacts with glucose in interstitial fluid
- Held by adhesive patch
- Replaced every 7-14 days

**Electrode system**:
- Electrochemical cell with multi-layered structure
- Working electrode
- Reference electrode (often silver/silver chloride)
- Counter electrode

**2. Transmitter**:
- Reusable or disposable device
- Clips on top of sensor patch
- Collects electrical signal from sensor
- Wirelessly sends data via Bluetooth to receiver/smartphone

**3. Receiver or Display Device**:
- Handheld receiver, smartphone app, or compatible insulin pump
- Displays real-time glucose level and trends
- Configured to provide alarms for high/low glucose readings

### B. Working Principle

**CGM uses amperometric biosensor**: Small electrical current generated in proportion to glucose concentration

**Step 1: Enzymatic reaction**:
- Glucose and oxygen from interstitial fluid diffuse into sensor through permeable membrane
- Glucose oxidase (GOx) catalyzes glucose oxidation
- **Reaction**: Glucose + O₂ → (GOx) → Gluconic acid + H₂O₂

**Step 2: Electrochemical oxidation**:
- Generated H₂O₂ diffuses to working electrode
- Constant voltage applied
- H₂O₂ electrochemically oxidized at electrode surface
- **Reaction**: H₂O₂ → O₂ + 2H⁺ + 2e⁻
- Releases electrons, produces oxygen and protons

**Step 3: Current measurement**:
- Electron flow creates measurable electrical current
- Current directly proportional to H₂O₂ oxidized
- This proportional to original glucose concentration in interstitial fluid

**Step 4: Signal processing and transmission**:
- Sensor's integrated circuit measures tiny electrical current
- Converts to digital glucose value
- Transmitter wirelessly sends data to display device

**Step 5: Display of results and trend analysis**:
- Receiver/app shows current glucose level
- Updates every 1-5 minutes
- Graphs historical data
- Shows glucose trends and speed of changes (trend arrows)
- More complete picture than single finger-prick test

**Step 6: Alerts and alarms**:
- Display device uses received data
- Triggers pre-set alerts for high/low glucose levels
- Helps user and healthcare providers take preventative action

---

## 9. DRAWBACKS OR LIMITATIONS OF SENSORS

**General sensor limitations:**

1. **Interference**:
   - Affected by temperature, humidity, electromagnetic fields
   - Can lead to inaccurate readings

2. **Calibration**:
   - Requires regular calibration for accuracy and reliability
   - Time-consuming
   - May require specialized equipment and expertise

3. **Drift**:
   - Readings become less accurate over time
   - Caused by aging of sensor components or environmental changes

4. **Cross-sensitivity**:
   - May respond to more than one type of gas or stimulus
   - Can lead to false readings if not properly accounted for

5. **Limited Lifespan**:
   - Need replacement after certain period
   - Results in additional costs and downtime

6. **Response Time**:
   - May have slow response
   - Particularly at low concentrations or rapidly changing conditions

7. **Cost**:
   - High-quality sensors can be expensive
   - Especially for specialized applications or high accuracy requirements

8. **Maintenance**:
   - May require regular cleaning or component replacement
   - Necessary to ensure proper operation

---

## SUMMARY OF KEY CONCEPTS

### 1. Sensors

**Definition**: Device converting physical/chemical quantities into electrical or optical signals

**Characteristics**: Selective, sensitive, accurate, reliable

**Selection criteria**: Selectivity, sensitivity, accuracy, calibration range, resolution, cost-effectiveness, repeatability

### 2. Classification

**Physical sensors**: Temperature, pressure, mechanical, optical, magnetic

**Chemical sensors**: Detect and measure chemical quantities

**Biological sensors**: Utilize biological materials/properties

**Electrochemical sensors**: Based on electrical property changes

**Radiation sensors**: Detect ionizing and non-ionizing radiation

### 3. Chemical Sensors

**Components**: Receptor (recognition system) + Transducer (physicochemical converter)

**Challenge**: Selectivity to target analyte among millions of species

**Applications**: Manufacturing monitoring, environmental sensing, health monitoring

### 4. Biosensors

**Three components**: Biological element + Transducer + Detector

**Biorecognition**: Enzymes, antibodies, nucleic acids, whole cells

**Transduction types**: Electrochemical, optical, mass-based, thermal

**Applications**: Medical diagnostics, glucose monitoring, drug screening

### 5. Gas Sensors

**Function**: Detect gas presence, convert to electrical signal

**Example**: Hydrogen sensors using catalytic bead, semiconductor, or metal oxide

**Catalytic bead mechanism**: Wheatstone bridge circuit measures resistance change from H₂ combustion

**Applications**: Industrial safety, environmental monitoring, healthcare, fire detection

### 6. Environmental and Medical Applications

**Environmental**: Air/water/soil quality monitoring

**Medical**: Blood glucose monitoring, breath analysis, drug/alcohol testing

### 7. Electrochemical Sensors

**Types**: Potentiometric (voltage), Amperometric (current), Conductometric (conductivity)

**Advantages**: High sensitivity, selectivity, low power consumption

**Example**: CGM sensor using amperometric biosensor with glucose oxidase enzyme

### 8. Sensor Limitations

**Common issues**: Interference, calibration needs, drift, cross-sensitivity, limited lifespan, response time, cost, maintenance requirements

---

## END OF SUMMARY

**Total Pages**: Approximately 15-18 pages when formatted

**Recommended Study Approach**:
1. Understand sensor fundamentals and definitions (Section 1)
2. Master sensor classification and types (Section 2)
3. Learn chemical sensor components and mechanisms (Section 3)
4. Study biosensor structure and working principles (Section 4)
5. Understand gas sensor types with hydrogen sensor example (Section 5)
6. Learn environmental and medical applications (Section 6)
7. Master electrochemical sensor classification table (Section 7)
8. Study CGM sensor as comprehensive example (Section 8)
9. Review sensor limitations (Section 9)
10. Focus on diagrams: Block diagrams for sensors, biosensors, gas sensors, CGM setup, Wheatstone bridge circuit

**Key Topics for Exam:**
- Sensor definition and characteristics
- Classification of sensors (all 5 types)
- Chemical sensor components (receptor + transducer)
- Biosensor three components and working principle
- Hydrogen gas sensor (catalytic bead) detailed mechanism
- Electrochemical sensor classification table
- CGM sensor complete working (6 steps)
- Applications in environmental monitoring and medical diagnostics
- Sensor limitations (8 points)

**Good luck with your studies!**