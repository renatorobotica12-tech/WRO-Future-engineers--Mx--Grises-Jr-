
- FINAL PLATFORM diagram


| System | Implementation |
|:---|:---|
| Steering | Ackermann steering geometry |
| Drive System | Rear-wheel drive |
| Main Controller | LEGO Mindstorms EV3 Brick |
| Coprocessors | 2 Arduino Nano, 1 for the camera and one for the PCB |
| Vision System | HuskyLens AI Camera |
| Distance Measurement | Five ultrasonic sensors |
| Communication | I²C protocol and UART protocol |
| Electronics | Custom-designed PCB |
| Control Algorithm | Adaptive Dual PD Controller |
| Decision System | Finite State Machine |


---

- QUICK SYSTEM OVERVIEW diagram

                 ┌──────────────────┐               ┌────────────────┐
                 │ HuskyLens Camera │               │   Ultrasonic   │
                 └────────┬─────────┘               │  Sensors (x5)  │
                          │                         └───────┬────────┘
                          │ UART                            │
                          ▼                                 ▼
                 ┌──────────────────┐               ┌────────────────┐
                 │   Arduino Nano   │               │   Custom PCB   │
                 │      (UART)      │               └───────┬────────┘
                 └────────┬─────────┘                       │
                          │                                 ▼
                          │                         ┌────────────────┐
                          │                         │  Arduino Nano  │
                          │                         │     (I²C)      │
                          │                         └───────┬────────┘
                          │                                 │
                          └────────────────┬────────────────┘
                                           │
                                           ▼
                                   ┌────────────────┐
                                   │    LEGO EV3    │
                                   │   Controller   │
                                   └────────┬───────┘
                                            │
                            ┌───────────────┴───────────────┐
                            ▼                               ▼
                    ┌──────────────┐                ┌──────────────┐
                    │Steering Motor│                │  Drive Motor │
                    └──────────────┘                └──────────────┘

---

- TEAM RESPONSABILITIES diagram

| Area | Renato | Paulina |
|:---|:---:|:---:|
| Mechanical Design | ✅ | ✅ |
| Robot Assembly | ✅ | ✅ |
| Electronics Integration | | ✅ |
| PCB Installation | ✅ | ✅ |
| Software Development | ✅ | |
| EV3 Programming | ✅ | |
| Arduino Programming | ✅ | |
| Documentation | ✅ | ✅ |
| Testing & Validation | ✅ | ✅ |

---

- ENGINEERING HIGHLIGHTS diagram

| Feature | Implementation |
|:---|:---|
| Steering System | Ackermann steering geometry |
| Drive System | Rear-wheel drive |
| Sensors | Five ultrasonic sensors |
| Vision | HuskyLens AI camera |
| Coprocessors | 2 Arduino Nano, 1 for camera and 1 for pcb |
| Electronics | Custom PCB |
| Communication | I²C architecture |
| Steering Calibration | Automatic encoder-based calibration |
| Control | Adaptive Dual PD controller |
| Navigation | Finite State Machine |
| Software | Modular architecture |
| Sensor Mounting | Custom 3D printed supports |
| Mechanical Design | Optimized weight distribution |
