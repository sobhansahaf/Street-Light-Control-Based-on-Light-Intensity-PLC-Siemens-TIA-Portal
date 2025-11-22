
# **Smart Street Lighting Control System**

This project implements a smart lighting system designed to improve **energy efficiency** and **road safety** by automatically controlling street lights based on **ambient light intensity** and **vehicle/pedestrian presence**. The system uses a comparator function to evaluate sensor inputs and switch between two operational modes: **Normal Mode** and **Power Saving Mode**.

---

## **Features**

* 🌤 **Automatic brightness-based lighting control**
* 🚶🚗 **Movement-activated lighting using PIR sensors**
* 🔄 **Two selectable modes: Normal / Power Saving**
* 💡 **Up to 4 lights with individual or grouped control**
* ⚡ **Enhanced energy efficiency through adaptive lighting**

---

## **Mode Selection**

Use the **selector switch** to choose between:

* **Normal Mode**
* **Power Saving Mode**

---

## **Normal Mode (Lumen-Based Control)**

In this mode, the system measures ambient brightness levels using a **light sensor**, and uses real-time lumen readings to determine how many lights should be turned on.

### **Light Behavior Based on Lumen Levels**

| Lumen Range  | Lights ON    | Behavior                        |
| ------------ | ------------ | ------------------------------- |
| **0 – 30**   | All 4 lights | Very dark, maximum illumination |
| **31 – 60**  | 2 lights     | Moderate low light              |
| **61 – 120** | 1 light      | Slightly dim environment        |
| **>120**     | 0 lights     | Sufficient ambient light        |

The system continuously evaluates brightness using a comparator function to adjust lighting accordingly.

---

## **Power Saving Mode (Motion-Based Control)**

In this mode, the system saves energy by activating lights **only when movement is detected**.

### **How It Works**

* Each of the **4 lights** has its own **PIR motion sensor**.
* When a vehicle or pedestrian is detected:

  * The corresponding light **turns ON**.
* When there is no motion:

  * The lights remain **OFF**.

This mode ensures lighting is delivered **on demand**, maximizing power savings without compromising safety.

---

## **System Components**

* Light Sensor (for lumen measurement)
* PIR Sensors (one per light)
* Comparator Circuit / Logic
* Selector Mode Switch
* 4 Lights (controlled individually)

---

## **Benefits**

* ⚡ **Significant energy savings**, especially in Power Saving Mode
* 👁‍🗨 **Improved visibility and safety** for pedestrians and drivers
* 🌱 **Environmentally friendly** operation
* 🔧 **Flexible configuration** based on lighting requirements

---

## **Usage**

1. Set the **selector switch** to your desired mode.
2. In **Normal Mode**, lighting will adjust automatically based on ambient brightness.
3. In **Power Saving Mode**, each light will activate only when its PIR sensor detects motion.


