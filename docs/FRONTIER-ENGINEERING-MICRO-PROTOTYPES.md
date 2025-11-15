# 📘 COMMONS FRONTIER ENGINEERING BLUE BOOK (VOLUME XVIII)

**Micro-Prototype Build Guides for Six Commons Technologies**

---

## PREFACE

This master document contains the stitched **Frontier Engineering Blue Book (Volume XVIII)** and six micro-prototype build books for:

1. **Aurora Mini Centrifuge**
2. **PFHMS Micro-Tile**
3. **BRL Soft-Limb Segment**
4. **CRTS Micro-Extruder Printer**
5. **MPRS Micro-Navigation Bot**
6. **CALEXS Micro-XR Pod**

Each build guide includes **beginner-level, step-by-step instructions**, materials lists, safety notes, and clear assembly procedures.

These micro-prototypes demonstrate the core physics and engineering principles behind each full-scale system using accessible, affordable materials that anyone can obtain.

---

## VOLUME XVIII: FRONTIER ENGINEERING FRAMEWORK

### 1. PURPOSE

A fully reality-grounded engineering framework demonstrating **micro-prototypes** that prove the physics, mechanics, materials, and system logic behind six Commons technologies.

**Why micro-prototypes?**
- Prove the core concepts at low cost
- Enable hands-on learning for students and makers
- Validate physics before investing in full-scale systems
- Democratize advanced technology education

**What these are NOT:**
- Not toys (they demonstrate real physics)
- Not production-ready (they're educational prototypes)
- Not shortcuts (they follow the same engineering principles as full systems)

---

### 2. SCIENTIFIC PRINCIPLES

This section outlines the **real-world physics** behind all six prototypes.

#### 2.1 Centripetal Force (Aurora Mini)

**Physics:** Artificial gravity is produced by rotation using the formula **a = ω²r**
- ω (omega) = angular velocity in radians/second
- r = radius from center of rotation
- a = centripetal acceleration (feels like gravity)

**Micro-prototype demo:** A bucket on a string spinning creates outward force. Water stays in the bucket even when upside-down at the top of the arc - this is the same principle used in space station designs.

#### 2.2 Shear-Thickening Fluids (PFHMS)

**Physics:** Non-Newtonian fluids change viscosity under stress. Cornstarch-water mixture acts as a liquid when still but hardens instantly when struck.

**Micro-prototype demo:** A plastic bag filled with cornstarch slurry between fabric layers creates a simple impact-hardening armor tile. Demonstrates the same principle as professional shear-thickening armor gel.

#### 2.3 Self-Healing Polymers (BRL)

**Physics:** Certain polymer chains can reform bonds after being cut, through hydrogen bonding or reversible cross-linking.

**Micro-prototype demo:** DIY slime (PVA glue + borax) or commercial "thinking putty" slowly reseals after small cuts, demonstrating polymer chain reformation.

#### 2.4 Multi-Material Extrusion (CRTS)

**Physics:** Controlled deposition of viscous materials through precision nozzles, with layer-by-layer additive construction.

**Micro-prototype demo:** A syringe controlled by stepper motor can precisely deposit frosting, gel, or clay paste in programmed patterns.

#### 2.5 Navigation Logic (MPRS)

**Physics:** Autonomous navigation requires sensing (detecting obstacles), decision-making (path planning), and actuation (motor control).

**Micro-prototype demo:** Obstacle detection sensors + microcontroller + motor control = basic SLAM-like decision-making and pathfinding.

#### 2.6 XR Immersion (CALEXS)

**Physics:** Multi-sensory integration creates presence. Combining visual (VR), haptic (vibration), audio, and biometric feedback produces immersive experiences.

**Micro-prototype demo:** Cardboard VR + phone + rumble motors + simple sensors = basic immersive environment demonstrating multi-modal sensory integration.

---

### 3. SYSTEM ARCHITECTURE

Each system has its own simplified architecture for micro-prototyping.

#### 3.1 Aurora Architecture (Micro)
```
Components:
├── Rotating chamber (bucket or bowl)
├── Axle + spin mechanism (string or motor)
├── Test mass (water or small object)
└── Observation window (clear side or marked rotation point)
```

#### 3.2 PFHMS Tile Architecture (Micro)
```
Layers:
├── Outer flexible casing (fabric)
├── STF gel pocket (cornstarch slurry in sealed bag)
├── Stiffening grid (optional: thin wire or craft sticks)
└── Sensor node (optional: accelerometer)
```

#### 3.3 BRL Limb Architecture (Micro)
```
Components:
├── Flexible skeleton (drinking straws or wire)
├── Self-healing skin (thinking putty or DIY slime)
├── Conductive paths (aluminum foil strips)
└── Pressure sensor (optional: resistive touch sensor)
```

#### 3.4 CRTS Extruder Architecture (Micro)
```
Components:
├── Frame (cardboard or wood base)
├── Stepper motor (28BYJ-48 with driver)
├── Syringe extruder (10-60mL medical syringe)
└── Material cartridge (frosting, gel, clay)
```

#### 3.5 MPRS Bot Architecture (Micro)
```
Components:
├── Two-wheel chassis (toy car or robot kit)
├── Distance sensors (HC-SR04 ultrasonic × 2)
├── Microcontroller (Arduino Uno or Nano)
└── Battery pack (4× AA or 9V)
```

#### 3.6 CALEXS Pod Architecture (Micro)
```
Components:
├── Booth frame (cardboard box or PVC)
├── Phone VR headset (Google Cardboard)
├── Haptic feedback (vibration motor × 4)
└── Audio system (headphones)
```

---

## BUILD BOOK 1: AURORA MINI CENTRIFUGE

### Overview

Build a hand-powered or motor-driven centrifuge that demonstrates artificial gravity through rotation.

**Difficulty:** Beginner  
**Time:** 30-60 minutes  
**Cost:** $5-$25

---

### Materials List

**Basic Version (Hand-Powered):**
- [ ] Sturdy bucket or bowl (1-2L capacity)
- [ ] Rope or strong string (1.5-2m)
- [ ] Water or small test mass
- [ ] Masking tape (for markers)
- [ ] Optional: Small sealed container for test object

**Advanced Version (Motorized):**
- [ ] Same as basic, plus:
- [ ] DC motor (12V, 100+ RPM)
- [ ] Power supply or battery pack
- [ ] Motor mount/bracket
- [ ] Bearing or smooth shaft

---

### Safety Notes

⚠️ **IMPORTANT SAFETY WARNINGS:**
1. **Clear area:** Ensure 3-meter radius is clear of people and fragile objects
2. **Structural integrity:** Check bucket/rope for cracks before each use
3. **Secure grip:** Never release while spinning
4. **Start slow:** Gradually increase speed to test stability
5. **Adult supervision:** Required for anyone under 16
6. **Outdoor use:** Perform outside or in large open space

---

### Assembly Instructions

#### Step 1: Prepare the Bucket
1. Choose a sturdy bucket with secure handle
2. Check for cracks or weak points
3. Mark center bottom with tape (observation point)
4. Add 100-500mL water (don't overfill)

#### Step 2: Attach Rope
1. Tie rope securely to bucket handle
2. Use bowline knot or double figure-eight
3. Test knot with gentle pulling
4. Ensure rope is at least 1.5m long

#### Step 3: Test Rotation
1. Hold rope end firmly with both hands
2. Start with slow arm circles
3. Gradually increase speed
4. Observe water behavior through bucket sides

#### Step 4: Demonstrate Centripetal Force
1. Once spinning steadily, tilt motion so bucket goes overhead
2. Water stays in bucket even when upside-down
3. This demonstrates centripetal acceleration mimicking gravity
4. Slowly decrease speed to stop

---

### Physics Explanation

**What's happening:**
- Centripetal acceleration creates "artificial gravity" pushing water outward
- From water's perspective, it feels pressed against bucket bottom
- Formula: a = v²/r where v = tangential velocity, r = radius
- At ~2 rotations/second with 1m rope, you create ~1.6g of acceleration

**Real-world application:**
- Space station rotating habitats use this same principle
- Larger radius = gentler rotation for same gravity
- Full-scale Aurora system uses controlled motors for precise rotation

---

### Experimentation Ideas

1. **Vary water amount:** How does weight affect ease of rotation?
2. **Add test objects:** Float a small sealed container - does it "fall" to bucket bottom?
3. **Measure RPM:** Count rotations and calculate centripetal acceleration
4. **Compare radii:** Try different rope lengths, note required speed for stability

---

### Upgrades

- Add motor mount for consistent rotation speed
- Install accelerometer to log actual g-forces
- Use clear bucket to better observe water behavior
- Create nested buckets to demonstrate radiation shielding mass

---

## BUILD BOOK 2: PFHMS MICRO-TILE

### Overview

Build a small impact-hardening armor tile using shear-thickening fluid (cornstarch mixture).

**Difficulty:** Beginner  
**Time:** 45 minutes (plus drying time)  
**Cost:** $8-$15

---

### Materials List

**For One 4"×4" Tile:**
- [ ] Cornstarch (1 cup / 120g)
- [ ] Water (½ cup / 120mL)
- [ ] Fabric squares (2× 15cm, canvas or denim)
- [ ] Ziplock bag (sandwich size, heavy-duty)
- [ ] Scissors
- [ ] Mixing bowl and spoon
- [ ] Duct tape or fabric glue
- [ ] Optional: Thin wire or craft sticks (for stiffening grid)
- [ ] Optional: Small zip ties (for quilting pattern)

---

### Safety Notes

⚠️ **Safety reminders:**
1. Non-toxic materials, but don't ingest mixture
2. Cornstarch can be slippery - clean spills immediately
3. Test impacts on soft surface first
4. Don't rely on this for real protection - educational demo only

---

### Assembly Instructions

#### Step 1: Mix Shear-Thickening Fluid
1. Pour 1 cup cornstarch into bowl
2. Slowly add ½ cup water while stirring
3. Mix until consistency of thick honey
4. Test: should pour slowly but harden when slapped
5. Adjust: add cornstarch if too runny, water if too thick

**Correct consistency test:**
- Stir slowly: mixture flows like liquid
- Slap surface: hand bounces off solid-like surface
- Release pressure: returns to liquid state

#### Step 2: Fill Bag
1. Open ziplock bag fully
2. Pour cornstarch mixture into bag
3. Remove air bubbles by gently pressing
4. Seal bag completely (check seal twice)
5. Trim excess plastic around sealed edge

#### Step 3: Create Fabric Envelope
1. Place one fabric square flat on table
2. Center sealed bag on fabric
3. Place second fabric square on top
4. Align edges of both fabric pieces

#### Step 4: Seal Edges
1. Use duct tape to seal all four edges, or
2. Fabric glue edges and let dry 2+ hours, or
3. Sew edges with simple running stitch

#### Step 5: Optional Enhancements
1. **Add stiffening grid:** Glue thin craft sticks to one side in cross pattern
2. **Create zones:** Use zip ties through fabric to create quilted pockets
3. **Stack layers:** Make 2-3 tiles and stack for increased protection

---

### Testing Protocol

#### Test 1: Hand Impact
1. Place tile on soft surface (pillow or foam)
2. Gently press with finger - should feel soft
3. Slap tile sharply - should feel hard resistance
4. Note how quickly it softens after impact (~1 second)

#### Test 2: Drop Test
1. Hold tile horizontal
2. Drop from waist height onto tile surface
3. Observe energy absorption (tile shouldn't bounce)
4. Compare to dropping same object on bare foam

#### Test 3: Repeated Impact
1. Tap tile 20 times in rapid succession
2. Verify it stiffens each time
3. Check bag seal remains intact
4. Remix if cornstarch settles to one side

---

### Physics Explanation

**How it works:**
- Cornstarch particles suspended in water (colloid)
- Under slow pressure: particles slide past each other (liquid)
- Under impact: particles jam together (solid-like)
- Remove force: particles unjam (liquid again)

**Real-world application:**
- Professional STF armor uses silica nanoparticles in polymer
- Same physics, more refined materials
- Response time: <50 milliseconds
- Can reduce impact force by 35-60%

---

### Experimentation Ideas

1. **Vary ratios:** Try different cornstarch:water ratios (2:1, 3:2, 1:1)
2. **Temperature:** Test in fridge vs. room temp - does behavior change?
3. **Impact force:** Measure how hard you can hit before cornstarch bag ruptures
4. **Comparison:** Make control tile with just water - how different is protection?

---

### Maintenance

- **Storage:** Keep flat, room temperature
- **Lifespan:** 2-4 weeks before cornstarch settles permanently
- **Refresh:** Knead bag to remix if separation occurs
- **Disposal:** Cornstarch mixture safe to compost or trash

---

## BUILD BOOK 3: BRL SOFT-LIMB SEGMENT

### Overview

Build a flexible limb segment with self-healing "skin" and simple sensor integration.

**Difficulty:** Intermediate  
**Time:** 1-2 hours  
**Cost:** $10-$20

---

### Materials List

**For One 6" Segment:**
- [ ] Self-healing putty (Thinking Putty) OR DIY slime kit (PVA glue + borax)
- [ ] Flexible skeleton: 3-4 drinking straws or pipe cleaners
- [ ] Conductive material: aluminum foil strips OR copper tape
- [ ] Optional sensor: Piezo buzzer or resistive touch sensor
- [ ] Optional actuator: Small servo motor (SG90)
- [ ] Fishing line or thin string (for cable actuation)
- [ ] Cardboard base (for mounting)
- [ ] Clear packing tape
- [ ] Optional: Multimeter (for conductivity testing)

---

### Safety Notes

⚠️ **Safety guidelines:**
1. DIY slime uses borax - keep away from eyes and mouth
2. Adult supervision required for borax handling
3. Wash hands after handling materials
4. Not intended for prosthetic use - demo only

---

### Assembly Instructions

#### Step 1: Build Flexible Skeleton
1. Take 3-4 drinking straws
2. Arrange parallel, spaced 1cm apart
3. Tape together at both ends with clear tape
4. Test flexibility - should bend smoothly
5. Mount to cardboard base at one end

#### Step 2: Add Conductive Pathways
1. Cut aluminum foil into 1cm × 15cm strips
2. Tape one strip along each straw (outside)
3. Leave 2cm exposed at both ends (contact points)
4. These act as "nerves" to detect electrical continuity

#### Step 3: Prepare Self-Healing Skin

**Option A - Commercial putty:**
1. Warm Thinking Putty in hands
2. Stretch into thin sheet (3-5mm thick)
3. Ready to wrap around skeleton

**Option B - DIY slime:**
1. Mix 120mL PVA glue + 1 tsp borax solution
2. Knead until cohesive
3. Let rest 10 minutes
4. Stretch into thin sheet

#### Step 4: Wrap Skeleton
1. Lay skeleton flat on table
2. Place putty/slime sheet over skeleton
3. Gently wrap around straws
4. Smooth to cover conductive strips
5. Leave end contact points exposed

#### Step 5: Test Self-Healing
1. Use craft knife to make small 1cm cut in skin
2. Press cut edges together for 10 seconds
3. Wait 5-10 minutes
4. Gently try to pull apart - should resist
5. Full healing: 30 minutes to 2 hours (depending on material)

#### Step 6: Optional Sensor Integration
1. Connect multimeter to foil strip ends
2. Bend limb - resistance should change
3. Cut skin - conductivity should break
4. After healing - conductivity should restore

---

### Testing Protocol

#### Test 1: Flexibility
1. Bend segment through 0° to 90° range
2. Should move smoothly without cracking
3. Skin should stretch with skeleton

#### Test 2: Self-Healing Demonstration
1. Make 5mm cut in skin with blade
2. Start timer
3. Check healing every 10 minutes
4. Test strength by gentle pulling
5. Document healing time

#### Test 3: Conductivity Recovery
1. Connect multimeter to conductive strips
2. Note baseline resistance
3. Cut through skin (cutting foil strip)
4. Resistance should go to infinity (open circuit)
5. Press edges together
6. After healing, measure resistance again
7. Calculate % recovery

#### Test 4: Repeated Stress
1. Bend segment 20 times
2. Check for skin fatigue or tearing
3. Make cut and heal
4. Bend 20 more times
5. Assess durability after healing

---

### Physics Explanation

**How self-healing works:**
- Polymer chains in putty/slime have weak reversible bonds
- When cut, bonds break
- Pressing edges together allows chains to re-entangle
- Hydrogen bonds slowly reform across the cut
- Not as strong as original, but functional

**Real-world application:**
- Medical-grade self-healing polymers use similar chemistry
- Professional version: PDMS with dynamic cross-linkers
- Conductive inks: silver nanoparticles in self-healing matrix
- Potential for prosthetics that repair surface damage

---

### Experimentation Ideas

1. **Healing time vs. cut depth:** Does a deeper cut take proportionally longer?
2. **Temperature effects:** Does warm putty heal faster than cold?
3. **Conductivity mapping:** Create grid of foil to locate cuts automatically
4. **Actuation:** Add servo with fishing line to create active bending

---

### Upgrades

- **Cable actuation:** Install servo and fishing line for controlled bending
- **Pressure sensors:** Add resistive sensors for "touch" detection
- **Multiple segments:** Chain 3-4 segments for full limb prototype
- **Microcontroller:** Add Arduino to log sensor data and control movement

---

## BUILD BOOK 4: CRTS MICRO-EXTRUDER PRINTER

### Overview

Build a simple single-axis extruder that demonstrates programmable material deposition.

**Difficulty:** Intermediate  
**Time:** 2-3 hours  
**Cost:** $25-$45

---

### Materials List

**Essential Components:**
- [ ] Stepper motor: 28BYJ-48 with ULN2003 driver ($3-5)
- [ ] Arduino Uno or Nano ($5-15)
- [ ] Breadboard and jumper wires ($5)
- [ ] 10-30mL syringe (medical grade, new) ($2-4)
- [ ] M5 threaded rod (20cm length) ($2)
- [ ] 3D printed plunger adapter OR improvised coupling ($0-5)
- [ ] Cardboard or wood base (12" × 12") ($0-2)
- [ ] Zip ties or mounting brackets ($2)
- [ ] USB cable for Arduino ($3)
- [ ] Power supply: 5V 1A ($5)

**Extrusion Materials:**
- [ ] Cake frosting in piping bag
- [ ] Silicone caulk
- [ ] Clay paste
- [ ] Peanut butter or spreadable paste

---

### Safety Notes

⚠️ **Important warnings:**
1. Use NEW syringes only (never used medical waste)
2. Food extrusions: use food-safe syringe and materials
3. Keep fingers away from moving threaded rod
4. Unplug power when adjusting hardware
5. Adult supervision required for soldering/power connections

---

### Assembly Instructions

#### Step 1: Build Base Frame
1. Cut cardboard to 12" × 12" base
2. Mark center point
3. Create vertical support (cardboard strip folded)
4. Mount stepper motor at center top with zip ties

#### Step 2: Create Plunger Actuator
1. Attach threaded rod to stepper motor shaft
2. Use coupling or hot glue for secure connection
3. Thread rod should hang vertically downward
4. Test: motor rotation should turn rod

#### Step 3: Mount Syringe
1. Remove syringe plunger
2. Mount syringe barrel vertical below motor
3. Align so threaded rod can push plunger from above
4. Secure with zip ties or tape

#### Step 4: Wire Electronics
```
Arduino → Stepper Driver
Pin 8  → IN1
Pin 9  → IN2
Pin 10 → IN3
Pin 11 → IN4
5V     → VCC
GND    → GND
```

#### Step 5: Load Software
Upload this basic Arduino code:

```cpp
#include <Stepper.h>

const int stepsPerRevolution = 2048; // 28BYJ-48 is 2048 steps
Stepper myStepper(stepsPerRevolution, 8, 10, 9, 11);

void setup() {
  myStepper.setSpeed(10); // RPM
  Serial.begin(9600);
}

void loop() {
  Serial.println("Extruding...");
  myStepper.step(512); // Quarter turn = ~0.5mL extrusion
  delay(2000);
  
  Serial.println("Retracting...");
  myStepper.step(-512);
  delay(2000);
}
```

#### Step 6: Load Material
1. Remove syringe from mount temporarily
2. Fill syringe with frosting or paste
3. Reattach plunger
4. Mount back on frame
5. Position collection surface below nozzle

---

### Testing Protocol

#### Test 1: Manual Extrusion
1. Power system
2. Observe plunger movement
3. Should see material extruding steadily
4. Check for smooth motion (no jamming)

#### Test 2: Extrusion Rate Calibration
1. Mark material level in syringe
2. Run 10 rotation cycles
3. Measure material extruded (volume or weight)
4. Calculate mL per step

#### Test 3: Pattern Drawing
1. Move collection surface by hand
2. Create simple line pattern
3. Verify consistent bead width
4. Check for gaps or over-extrusion

#### Test 4: Material Comparison
1. Test with frosting (easy)
2. Test with caulk (medium)
3. Test with clay (hard)
4. Note required pressure differences

---

### Physics Explanation

**How it works:**
- Stepper motor provides precise rotation control
- Threaded rod converts rotation to linear motion
- Linear motion pushes syringe plunger
- Plunger pressure forces material through nozzle
- Deposition rate = motor speed × plunger advance

**Real-world application:**
- Professional 3D printers use same concept with heated nozzles
- Multi-material printers swap toolheads (like full CRTS system)
- QR traceability: log every motor command to track what was printed
- Full CRTS has XY gantry for 2D patterns, this demo shows Z-axis extrusion

---

### Experimentation Ideas

1. **Speed variation:** How does motor speed affect extrusion quality?
2. **Viscosity test:** Which materials extrude smoothly vs. clog?
3. **Add XY stage:** Move collection surface in programmed patterns
4. **Swap nozzles:** Try different syringe tip sizes
5. **Multi-material:** Use two syringes and switch between them

---

### Upgrades

- **Full XY motion:** Add second stepper for 2D gantry
- **Heated extruder:** Add heating element for thermoplastic extrusion
- **Multiple syringes:** Carousel system for material switching
- **Computer control:** Write G-code interpreter for pattern drawing
- **QR logging:** Add database to log extrusion parameters per print

---

## BUILD BOOK 5: MPRS MICRO-NAVIGATION BOT

### Overview

Build a simple two-wheeled robot that demonstrates autonomous obstacle avoidance.

**Difficulty:** Intermediate  
**Time:** 2-3 hours  
**Cost:** $30-$50

---

### Materials List

**Robot Chassis:**
- [ ] Two-wheel robot kit OR toy car chassis ($10-15)
- [ ] Two DC motors with wheels (if not in kit) ($8)
- [ ] Caster wheel or ball bearing (front support) ($2)
- [ ] Plastic or cardboard platform ($0-3)

**Electronics:**
- [ ] Arduino Uno or Nano ($8-15)
- [ ] L298N motor driver module ($5)
- [ ] HC-SR04 ultrasonic distance sensors (× 2) ($4)
- [ ] Breadboard and jumper wires ($5)
- [ ] Battery pack: 6× AA or 2× 18650 ($5-10)
- [ ] Battery holder and power switch ($3)

**Tools:**
- [ ] Screwdriver
- [ ] Zip ties or mounting screws
- [ ] USB cable for programming

---

### Safety Notes

⚠️ **Safety precautions:**
1. Never operate bot near stairs or edges
2. Test in clear, safe area first
3. Include kill switch for emergency stop
4. Keep clear of moving wheels during operation
5. Supervise operation at all times

---

### Assembly Instructions

#### Step 1: Assemble Chassis
1. If using kit: follow manufacturer instructions
2. If DIY: mount motors to cardboard platform
3. Attach wheels to motor shafts
4. Add caster wheel at front for balance
5. Test: should roll smoothly when pushed

#### Step 2: Mount Electronics
1. Secure Arduino to chassis with zip ties or tape
2. Mount motor driver near motors
3. Position battery pack at rear for weight balance
4. Leave room for sensor mounting at front

#### Step 3: Install Sensors
1. Mount two ultrasonic sensors at front
2. Angle slightly outward (15° each)
3. One sensor for left obstacle detection
4. One sensor for right obstacle detection
5. Height: 5-10cm above ground

#### Step 4: Wire Electronics

**Motor Driver Connections:**
```
Arduino → L298N
Pin 5 → ENA (left motor speed)
Pin 6 → ENB (right motor speed)
Pin 7 → IN1 (left motor direction)
Pin 8 → IN2 (left motor direction)
Pin 9 → IN3 (right motor direction)
Pin 10 → IN4 (right motor direction)

L298N → Motors
OUT1 → Left motor (+)
OUT2 → Left motor (-)
OUT3 → Right motor (+)
OUT4 → Right motor (-)

Power:
Battery + → L298N (12V)
Battery - → GND (common)
L298N 5V → Arduino VIN
```

**Sensor Connections:**
```
Left Sensor (HC-SR04):
VCC → 5V
GND → GND
Trig → Pin 2
Echo → Pin 3

Right Sensor:
VCC → 5V
GND → GND
Trig → Pin 4
Echo → Pin 11
```

#### Step 5: Upload Navigation Code

```cpp
// Pin definitions
#define TRIG_L 2
#define ECHO_L 3
#define TRIG_R 4
#define ECHO_R 11
#define ENA 5
#define ENB 6
#define IN1 7
#define IN2 8
#define IN3 9
#define IN4 10

const int SAFE_DISTANCE = 20; // cm

void setup() {
  pinMode(TRIG_L, OUTPUT);
  pinMode(ECHO_L, INPUT);
  pinMode(TRIG_R, OUTPUT);
  pinMode(ECHO_R, INPUT);
  pinMode(ENA, OUTPUT);
  pinMode(ENB, OUTPUT);
  pinMode(IN1, OUTPUT);
  pinMode(IN2, OUTPUT);
  pinMode(IN3, OUTPUT);
  pinMode(IN4, OUTPUT);
  Serial.begin(9600);
}

int getDistance(int trig, int echo) {
  digitalWrite(trig, LOW);
  delayMicroseconds(2);
  digitalWrite(trig, HIGH);
  delayMicroseconds(10);
  digitalWrite(trig, LOW);
  
  long duration = pulseIn(echo, HIGH);
  int distance = duration * 0.034 / 2;
  return distance;
}

void forward() {
  digitalWrite(IN1, HIGH);
  digitalWrite(IN2, LOW);
  digitalWrite(IN3, HIGH);
  digitalWrite(IN4, LOW);
  analogWrite(ENA, 150);
  analogWrite(ENB, 150);
}

void turnRight() {
  digitalWrite(IN1, HIGH);
  digitalWrite(IN2, LOW);
  digitalWrite(IN3, LOW);
  digitalWrite(IN4, HIGH);
  analogWrite(ENA, 150);
  analogWrite(ENB, 150);
}

void turnLeft() {
  digitalWrite(IN1, LOW);
  digitalWrite(IN2, HIGH);
  digitalWrite(IN3, HIGH);
  digitalWrite(IN4, LOW);
  analogWrite(ENA, 150);
  analogWrite(ENB, 150);
}

void stopMotors() {
  digitalWrite(IN1, LOW);
  digitalWrite(IN2, LOW);
  digitalWrite(IN3, LOW);
  digitalWrite(IN4, LOW);
}

void loop() {
  int distL = getDistance(TRIG_L, ECHO_L);
  int distR = getDistance(TRIG_R, ECHO_R);
  
  Serial.print("L: "); Serial.print(distL);
  Serial.print(" R: "); Serial.println(distR);
  
  if (distL > SAFE_DISTANCE && distR > SAFE_DISTANCE) {
    forward(); // Path is clear
  } 
  else if (distL < SAFE_DISTANCE && distR > SAFE_DISTANCE) {
    turnRight(); // Obstacle on left
  } 
  else if (distR < SAFE_DISTANCE && distL > SAFE_DISTANCE) {
    turnLeft(); // Obstacle on right
  } 
  else {
    turnRight(); // Both sides blocked, turn around
  }
  
  delay(100);
}
```

#### Step 6: Initial Testing
1. Place bot on floor in clear area
2. Power on battery pack
3. Observe initial movement
4. Hold hand in front of sensors
5. Bot should detect and turn away

---

### Testing Protocol

#### Test 1: Sensor Range
1. Place obstacle at various distances: 5cm, 10cm, 20cm, 30cm
2. Verify sensor readings match actual distance (±2cm)
3. Test with different obstacle materials (cardboard, metal, fabric)

#### Test 2: Obstacle Avoidance
1. Create simple obstacle course (boxes, books)
2. Place bot at start
3. Bot should navigate without collision
4. Measure success rate over 10 trials

#### Test 3: Navigation Path
1. Set up corridor with walls on both sides
2. Bot should drive down center
3. Test width: minimum 40cm for reliable navigation

#### Test 4: Battery Life
1. Fully charge batteries
2. Run continuous operation
3. Measure runtime until motors slow
4. Typical: 30-90 minutes depending on battery capacity

---

### Physics Explanation

**How it works:**
- **Ultrasonic sensors:** Emit 40kHz sound pulse, measure echo return time
- **Distance calculation:** Time × speed of sound ÷ 2 = distance
- **Decision logic:** If obstacle close → turn away; if clear → go forward
- **Differential drive:** Turn by running wheels at different speeds

**Real-world application:**
- Full MPRS uses LIDAR (laser scanning) instead of ultrasonic
- SLAM mapping builds memory of environment
- Professional version has payload bay and auto-docking
- This demo shows same decision-making logic at micro scale

---

### Experimentation Ideas

1. **Path memory:** Add code to remember previously tried directions
2. **Target seeking:** Add IR remote to create "goal" location
3. **Line following:** Add IR sensors below to follow black line
4. **Swarm behavior:** Build 2-3 bots that coordinate
5. **Mapping:** Log sensor readings and motor commands to visualize path

---

### Upgrades

- **LIDAR module:** Swap ultrasonic for 360° laser scanner
- **Camera:** Add Raspberry Pi with camera for vision-based navigation
- **IMU sensor:** Add gyroscope/accelerometer for precise turns
- **WiFi control:** Add ESP32 for remote monitoring and control
- **Payload delivery:** Add servo gripper to pick up and drop small objects

---

## BUILD BOOK 6: CALEXS MICRO-XR POD

### Overview

Build a simple immersive experience booth combining phone VR with haptic feedback.

**Difficulty:** Beginner-Intermediate  
**Time:** 2-4 hours  
**Cost:** $25-$60

---

### Materials List

**Structure:**
- [ ] Large cardboard box (refrigerator/wardrobe box) OR
- [ ] PVC pipe frame (10× 1m pipes + connectors) ($20)
- [ ] Black fabric or curtain (2m × 2m) ($10)
- [ ] Duct tape and zip ties ($5)

**Display:**
- [ ] Smartphone (your existing phone)
- [ ] Google Cardboard VR headset ($5-15)
- [ ] VR apps (free downloads: YouTube VR, Google Earth VR)

**Haptics:**
- [ ] Vibration motors: 4× phone vibration motors ($8)
- [ ] Arduino Nano ($5)
- [ ] Transistors: 4× 2N2222 ($2)
- [ ] Breadboard and wires ($5)
- [ ] 9V battery ($3)

**Audio:**
- [ ] Over-ear headphones or earbuds ($10-30)
- [ ] Optional: Small speaker for bass ($10)

**Optional Enhancements:**
- [ ] LED strip (5m, RGB) ($12)
- [ ] Desk fan (for wind effect) ($10)

---

### Safety Notes

⚠️ **Safety guidelines:**
1. **Motion sickness:** Start with short 5-minute sessions
2. **Exit access:** Keep one side open for easy exit
3. **Ventilation:** Ensure adequate airflow
4. **Trip hazards:** Keep floor clear inside booth
5. **Emergency stop:** Have someone outside to assist if needed

---

### Assembly Instructions

#### Step 1: Build Booth Frame

**Option A - Cardboard Box:**
1. Obtain large box (1m × 1m × 2m ideal)
2. Cut entrance opening on one side (0.8m wide)
3. Line interior with black fabric to reduce light
4. Reinforce corners with duct tape

**Option B - PVC Frame:**
1. Build cube frame: 1m × 1m × 2m
2. Use PVC connectors at corners
3. Drape black fabric over three sides
4. Leave one side open as entrance

#### Step 2: Install Haptic Floor
1. Cut cardboard square to fit booth floor
2. Tape vibration motors to underside at four corners
3. Cover motors with thin foam padding
4. User stands/sits on floor to feel vibrations

#### Step 3: Wire Haptic System

**Circuit for Each Motor:**
```
Arduino Pin → Transistor Base (through 1kΩ resistor)
Transistor Collector → Motor (+)
Transistor Emitter → GND
9V Battery (+) → Motor (+)
```

**Arduino Code:**
```cpp
int motors[4] = {3, 5, 6, 9}; // PWM pins

void setup() {
  for(int i=0; i<4; i++) {
    pinMode(motors[i], OUTPUT);
  }
  Serial.begin(9600);
}

void loop() {
  // Example: Rumble all motors
  for(int i=0; i<4; i++) {
    analogWrite(motors[i], 200); // 0-255 intensity
  }
  delay(500);
  
  // Stop
  for(int i=0; i<4; i++) {
    analogWrite(motors[i], 0);
  }
  delay(500);
  
  // You can create patterns:
  // Waves, corners, rhythms, etc.
}
```

#### Step 4: Set Up VR System
1. Download VR apps to phone (YouTube VR, InCell VR, etc.)
2. Insert phone into Cardboard headset
3. Adjust lenses for clear focus
4. Connect headphones to phone

#### Step 5: Optional Lighting
1. Install LED strip around booth interior perimeter
2. Connect to separate Arduino or LED controller
3. Program color changes to sync with VR content

#### Step 6: Create Entry/Exit
1. Mark entrance clearly
2. Add small shelf outside for phone/headset prep
3. Place chair or cushion inside for sitting

---

### Testing Protocol

#### Test 1: Comfort Assessment
1. Enter booth and sit
2. Put on VR headset
3. Stay for 5 minutes
4. Check for:
   - Adequate space
   - Good ventilation
   - Comfortable seating
   - Easy exit

#### Test 2: Haptic Sync Test
1. Play video with rhythm (music video)
2. Manually trigger haptics to match beats
3. Verify vibrations felt clearly through floor
4. Adjust motor intensity as needed

#### Test 3: Immersion Evaluation
1. Try 3-4 different VR experiences
2. Rate immersion level (1-10 scale)
3. Identify improvements needed
4. Test with 2-3 different people for feedback

#### Test 4: Motion Sickness Check
1. Start with 5-minute session
2. Monitor for dizziness or nausea
3. If comfortable, extend to 10-15 minutes
4. Never exceed 30 minutes for first-time users

---

### Physics Explanation

**How it works:**
- **VR headset:** Dual lenses create stereoscopic 3D effect
- **Head tracking:** Phone sensors (gyro/accel) detect head rotation
- **Haptic feedback:** Vibrations simulate touch/movement sensations
- **Multi-sensory integration:** Brain combines visual + tactile + audio → presence
- **Immersion:** Blocking external stimuli increases sense of "being there"

**Real-world application:**
- Full CALEXS pod has 3× large screens or projectors
- 12-zone haptic floor with precise vibration control
- Biometric sensors (heart rate, galvanic skin response)
- Used for therapy (PTSD, phobias), education, training
- This micro version demonstrates same multi-sensory principles

---

### Experimentation Ideas

1. **Content pairing:** Which VR experiences work best with haptics?
2. **Haptic patterns:** Create library of patterns (explosion, rain, footsteps)
3. **Scent addition:** Use essential oil diffuser for smell dimension
4. **Wind effects:** Add fan for airflow during flight simulations
5. **Social presence:** Add external monitor so others can see VR view

---

### Experience Suggestions

**Educational:**
- Google Earth VR: Explore world landmarks with location-based haptics
- Space tours: Rumble during rocket launch sequences
- Ocean dives: Wave patterns on floor sync with underwater movement

**Therapeutic:**
- Relaxation environments: Gentle haptics for meditation
- Exposure therapy: Controlled anxiety scenarios with support
- Mindfulness: Focus exercises with biofeedback (if sensors added)

**Entertainment:**
- Roller coaster simulations: Strong haptics for motion
- Rhythm games: Beat matching with floor vibrations
- 360° videos: Enhanced immersion with environmental effects

---

### Upgrades

- **Rumble seat:** Add chair with bass shakers
- **3-screen setup:** Use projectors on walls instead of phone VR
- **Biometric sensors:** Add heart rate monitor with Arduino logging
- **Scent module:** Install programmable scent diffuser
- **Lighting sync:** DMX-controlled RGB lights respond to VR content
- **Computer control:** Use PC VR (Oculus Rift, HTC Vive) for higher quality

---

## APPENDIX A: SAFETY MATRIX

| Build | Primary Hazards | Mitigation | Supervision |
|-------|----------------|------------|-------------|
| Aurora | Flying bucket, water spill | Clear area, slow start | Required |
| PFHMS | None (non-toxic) | Clean spills | Optional |
| BRL | Borax (if DIY slime) | Avoid ingestion, wash hands | Required for <16 |
| CRTS | Moving parts | Keep fingers clear, power off when adjusting | Recommended |
| MPRS | Moving robot, edges | Test in safe area, padding on edges | Required for <12 |
| CALEXS | Motion sickness | Short sessions, easy exit | Recommended |

---

## APPENDIX B: MATERIALS SOURCING

### Budget Options

**Under $50 total (pick one):**
- Aurora (hand-powered): $5
- PFHMS: $12
- BRL: $15
- CALEXS (basic): $25

**Under $100 total (pick two):**
- PFHMS + BRL: $27
- Aurora + PFHMS: $17
- BRL + CALEXS: $40

**Complete set:** $120-$180 for all six micro-prototypes

### Suppliers

**Electronics:**
- Arduino: arduino.cc, Adafruit, SparkFun
- Sensors/motors: Amazon, AliExpress, eBay

**Materials:**
- Cornstarch: grocery store
- Thinking Putty: Crazy Aaron's (toy stores)
- Fabric: craft stores (Joann, Michaels)

**Hardware:**
- PVC pipe: hardware stores (Home Depot, Lowe's)
- Syringes: pharmacy or medical supply
- Cardboard: ask at appliance stores (free)

---

## APPENDIX C: EDUCATIONAL STANDARDS ALIGNMENT

These micro-prototypes align with:

**NGSS (Next Generation Science Standards):**
- MS-PS2-2: Plan investigation of motion forces
- MS-PS3-5: Energy transfer and transformation
- HS-ETS1-2: Design solution to complex problem

**STEM Skills:**
- Engineering design process
- Prototyping and iteration
- Data collection and analysis
- Materials science
- Programming fundamentals

**Suitable for:**
- Middle school (grades 6-8) with supervision
- High school (grades 9-12) independent projects
- Maker spaces and STEM clubs
- Science fairs and competitions
- College intro engineering courses

---

## APPENDIX D: TROUBLESHOOTING

### Aurora Issues

**Problem:** Water spills during spin  
**Solution:** Start slower, ensure bucket has no cracks, use less water

**Problem:** Rope slips from handle  
**Solution:** Use bowline knot, add tape to handle for grip

---

### PFHMS Issues

**Problem:** Cornstarch mixture too liquid  
**Solution:** Add more cornstarch gradually, 1 tablespoon at a time

**Problem:** Bag leaks  
**Solution:** Use heavy-duty freezer bags, seal with tape over zipper

**Problem:** Tile doesn't harden on impact  
**Solution:** Remix thoroughly, ensure 2:1 cornstarch:water ratio

---

### BRL Issues

**Problem:** Slime too sticky  
**Solution:** Knead more, let rest 10 minutes, add tiny bit of borax

**Problem:** Putty won't heal cuts  
**Solution:** Ensure edges pressed firmly together, wait longer (putty heals slower than slime)

**Problem:** Conductivity not restoring  
**Solution:** Foil strips must be in direct contact, not separated by thick putty layer

---

### CRTS Issues

**Problem:** Motor not moving  
**Solution:** Check wiring, verify power supply, test motor separately

**Problem:** Material not extruding  
**Solution:** Check for clogs, ensure material not too thick, verify plunger alignment

**Problem:** Inconsistent extrusion  
**Solution:** Slow motor speed, use more viscous material, clean nozzle

---

### MPRS Issues

**Problem:** Bot doesn't move  
**Solution:** Check motor connections, verify battery charge, test motors with separate power

**Problem:** Sensors not detecting obstacles  
**Solution:** Check wiring, verify sensor height (not too low), ensure nothing blocking sensor faces

**Problem:** Bot drives in circles  
**Solution:** Adjust motor speeds to be equal, check wheel alignment, verify both motors functional

**Problem:** Erratic behavior  
**Solution:** Lower motor speeds, increase delay between sensor readings, check for loose wires

---

### CALEXS Issues

**Problem:** Motion sickness  
**Solution:** Shorten session length, increase ventilation, try different VR content

**Problem:** Haptics not felt  
**Solution:** Increase motor voltage (up to 9V max), remove excess padding, verify motor function

**Problem:** Phone overheating  
**Solution:** Better ventilation, shorter sessions, close background apps, don't charge while in use

**Problem:** Blurry VR image  
**Solution:** Adjust lens position, clean lenses, ensure phone screen clean, verify app resolution settings

---

## APPENDIX E: PROGRESSION PATH

### From Micro to Professional

This chart shows how each micro-prototype relates to the professional system:

| Micro-Prototype | Professional System | Scale Factor | Key Differences |
|----------------|---------------------|--------------|-----------------|
| Hand-spun bucket | Aurora Mini Centrifuge | 1:5 size | Motors, pressure vessel, safety systems |
| Cornstarch tile | PFHMS v2.0 Tile | 1:2 size | Industrial STF, SMA, MCU logging |
| Putty limb | BRL Soft-Limb | 1:3 size | Medical-grade PDMS, precision sensors, actuation |
| Syringe extruder | CRTS Multi-Material | 1-axis vs. 3-axis | XY gantry, heated bed, multi-head carousel |
| Obstacle avoider | MPRS Navigation Bot | Basic vs. advanced | LIDAR, SLAM mapping, payload system |
| Cardboard booth | CALEXS XR Pod | 1:4 scale | Multi-screen, 12-zone haptics, biometrics |

### Learning Progression

1. **Build micro-prototype** (this document)
2. **Master physics principles** (understand why it works)
3. **Study professional specs** (Volume XVIII, Blue Book)
4. **Identify upgrade path** (what changes needed)
5. **Source professional components** (BOMs in Volume XVIII)
6. **Build intermediate version** (half-scale or partial features)
7. **Construct full prototype** (following engineering Blue Book)

---

## CONCLUSION

These six micro-prototypes prove that the Commons technologies are based on **real, achievable physics**. Anyone with basic tools and modest budget can demonstrate:

✅ **Artificial gravity** through centripetal force  
✅ **Impact-hardening materials** via shear-thickening fluids  
✅ **Self-healing polymers** with reversible chemistry  
✅ **Multi-material fabrication** through programmable extrusion  
✅ **Autonomous navigation** with sensor-based decision making  
✅ **Immersive XR experiences** via multi-sensory integration  

The gap between these micro-prototypes and full professional systems is **engineering refinement**, not impossible physics. Every component in the professional systems (Volume XVIII) can be purchased from commercial suppliers and assembled using standard manufacturing techniques.

**These are not science fiction concepts. These are engineering projects.**

---

## CREDITS & LICENSING

**Commons Frontier Engineering Blue Book (Volume XVIII)**  
**Micro-Prototype Build Guides**

Published: 2025-11-15  
License: Creative Commons BY-SA 4.0  
Attribution: Commons Engineering Council

**Safety Disclaimer:** These are educational prototypes. They demonstrate physical principles but are not production-ready devices. Follow all safety guidelines. Adult supervision required for builders under 16. Not responsible for injuries or damages from improper construction or use.

**Educational Use:** These guides may be freely shared for non-commercial educational purposes. Commercial use requires attribution and share-alike licensing.

---

**End of Volume XVIII: Frontier Engineering Blue Book**

For professional engineering specifications, see:
- Volume XVIII: Engineering Validation
- Commons Blue Book: Engineering Baseline
- Agent Review Packet: Verification Standards
