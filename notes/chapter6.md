# Chapter 6 — Automated and Emerging Technologies (Short Notes)

**Cambridge IGCSE & O Level Computer Science** · Quick revision notes
Sections: **6.1** Automated systems · **6.2** Robotics · **6.3** Artificial Intelligence (AI)

---

# 6.1 Automated systems

## 6.1.1 Sensors, microprocessors and actuators

An **automated system** is a combination of software and hardware (sensors, microprocessors, actuators) designed to work **automatically without human intervention** (though often with human monitoring). The basic loop:

1. **Sensors** — input devices that take readings from the surroundings and send data to the microprocessor. Analogue data is first converted by an **ADC** (analogue-to-digital converter).
2. **Microprocessor** — processes the data and decides what action to take (based on programming, often comparing with stored data in a database).
3. **Actuators** — receive output signals and operate motors, valves, pumps, pistons, etc. (A **DAC** converts digital signals back to analogue where needed.)

## 6.1.2 Application areas (advantages & disadvantages)

Automated systems are used in **industry, transport, agriculture, weather, gaming, lighting and science**.

**General advantages** (recur across examples): faster reaction than humans; safer (keeps humans from danger, timely action); runs at optimum conditions; cheaper long-term (fewer staff); higher productivity; more consistent/repeatable results.

**General disadvantages**: expensive to set up and test; unforeseen conditions may not have been tested (hence a human **supervisor**); vulnerable to **cyberattacks**; high/specialist maintenance costs; possible **deskilling** and unemployment.

**Industrial** — e.g. a **nuclear power station** controlled by a **Distributed Control System (DCS)**, or **paracetamol manufacture**. Sensors send data to a central computer/DCS, which checks a database and signals actuators (pumps, valves, heaters). A supervisor in a remote room can **override** the system.

**Transport** — automatic train signal control (stops train at red light); aircraft **autopilot** controlling flaps, throttle and rudder.
- **Self-parking cars:** bumper sensors act as transmitters/receivers; signal bounce-back time builds a **3D image**; computer controls steering, brakes and throttle. *Pros:* fit smaller spaces, fewer dents, safer. *Cons:* over-reliance/deskilling, dirty/faulty sensors, kerbing low kerbs, expensive.
- **Adaptive cruise control:** driver sets a speed; lasers measure the distance to the car ahead; if too close, the computer signals actuators to brake/reduce throttle, otherwise adjusts to the set speed.

**Agriculture** — e.g. **Brazil irrigation system**: ultrasonic water-level sensors + automatic weather station data sent wirelessly to a controller, which starts/stops water pumps via actuators; a supervisor oversees remotely. *Pros:* low labour, efficient water use, fast, safe, different crops handled at once. *Cons:* expensive, high maintenance, blocked channels not detected.

**Weather stations** — gather data in remote areas. Components: microprocessor, storage (database), battery (often solar), wireless transmitter, and sensors:

| Sensor | Measures |
|---|---|
| Thermometer | Temperature |
| Anemometer | Wind speed |
| Hygrometer | Humidity |
| Barometer | Air pressure |
| Level sensor | Rainfall |
| Light sensor | Hours of daylight |

The only actuator is in the **tipping-bucket rain gauge**. Some stations send reports to pilots every five minutes.

**Gaming** — sensors add realism: **accelerometers** (detect tilting/acceleration) and **proximity sensors** (detect hand/finger position on touch pads). With a microcontroller these give immersive interaction.

**Lighting** — uses **light sensors** (ambient light), **motion sensors** (turn on when someone enters) and **infrared sensors** (motion/security). *Pros:* automatic control, less energy, longer bulb life, programmable displays. *Cons:* expensive, wireless less reliable, maintenance.

**Science** — e.g. a **chemical laboratory experiment**: level sensors and a colorimeter feed a microprocessor that opens/closes a tap via an actuator. *Pros:* consistent, safer, faster (parallel experiments), automatic analysis, fewer staff, remote monitoring. *Cons:* less flexible than humans, security risks if data shared, expensive.

**AI in automated systems** — *Advantages:* stores vast facts, learns from huge data, spots patterns humans miss. *Disadvantages:* changes the skill set, and is only as good as the data it is trained on.

---

# 6.2 Robotics

## 6.2.1 What is robotics?

**Robotics** is the branch of (computer) science covering the **design, construction and operation of robots**. (The word "robot" comes from the Czech *robota* = "forced labour".)

**Asimov's three laws of robotics:** (1) a robot may not injure a human through action or inaction; (2) a robot must obey humans, unless this conflicts with law 1; (3) a robot must protect itself, unless this conflicts with law 1.

Robots are found in **factories** (welding, spray-painting, cutting, bottling, warehouses), **the home** (vacuum cleaners, lawn mowers, window/pool cleaners, entertainment), and as **drones** (UAVs for reconnaissance or deliveries).

**Software robots are NOT true robots:** e.g. **search bots/WebCrawlers** (scan and categorise websites) and **chatbots** (converse with users).

| Independent robot | Dependent robot |
|---|---|
| **No direct human control** (autonomous). | Has a **human interface** (computer/control panel). |
| Can **totally replace** human activity. | **Supplements** rather than replaces humans. |

## 6.2.2 Characteristics of a robot

To be a true robot, a device must have all three:

1. **Sense its surroundings** — via sensors (light, pressure, temperature, acoustic…) feeding a microprocessor.
2. **A degree of movement** — wheels, cogs, pistons, gears, motors, hydraulics; uses **end-effectors** (interchangeable attachments for welding, spraying, cutting, gripping).
3. **Programmable** — has a **controller** (its "brain") that decides actions, programmable for different tasks.

> Robotics and AI are largely **separate** fields — many robots have **no AI** because they do repetitive tasks rather than adapting.

## 6.2.3 Roles of robots, with advantages and disadvantages

**Industry** — paint spraying, welding, microchip and goods manufacture, automatic warehouses. Programmed either by a sequence of instructions or by recording a human operator's movements (guiding the arm, or wearing sensors).

| Advantages | Disadvantages |
|---|---|
| Work in hazardous conditions; 24/7; cheaper long-term; higher productivity; more consistent; better at repetitive/boring tasks; lower heat/light costs. | Struggle with non-standard tasks; cause unemployment/deskilling; factories may move abroad; expensive to buy and set up. |

**Transport** — driverless vehicles (the big barrier is **human perception**, not technology):
- **Autonomous cars/buses:** radar, ultrasonics and cameras act as the "eyes and ears", building a **3D image**; the microprocessor signals actuators to steer, brake, change gear. *Pros:* safer (no human error), greener, less congestion, more lane capacity, less commuting, self-parking. *Cons:* expensive, hacking fear, software glitches, maintenance/clean cameras, user reluctance, job losses.
- **Autonomous trains:** use **LiDaR** (lasers building a 3D image), proximity/infrared sensors, cameras, GPS and actuators. *Pros:* punctual, lower running costs, safer, energy-efficient, more frequent, easy rescheduling. *Cons:* hacking, struggles with very busy services, high capital cost, passenger behaviour/reluctance, need for CCTV.
- **Autonomous (unpiloted) airplanes:** sensors for turbulence/depressurisation, self-testing, GPS, actuators for throttle/flaps/rudder. *Pros:* comfort, lower costs, safer (fewer pilot errors), better aerodynamics. *Cons:* security/terrorism, hard-to-handle emergencies, hacking, glitches, reluctance.

**Agriculture** (population pressure drives automation):
- **Harvesting/picking** — faster, more accurate (only ripe produce), higher yields (e.g. *vegebot*'s cameras).
- **Weed control** — distinguishes weed from crop using **AI**; uses **GPS** tracking and a blade actuator.
- **Phenotyping** — observing a plant's physical traits to assess health/growth using sensors, thermal cameras and **machine learning**.
- **Seed-planting & fertiliser drones** — aerial images for accurate planting/spraying; even **cloud seeding** with silver iodide.
- **Autonomous devices** — grass cutters, weeding/pruning/harvesting/seeding robots using sensors and cameras.

**Medicine** — surgery (safer, quicker, cheaper), patient monitoring, room disinfecting, blood sampling (less painful, safer for staff), **microbots** for targeted drug therapy, and robotic **prosthetic limbs** (bionic skins/neural implants giving feedback).

**Domestic** — autonomous vacuum cleaners and grass cutters (proximity sensors, cameras, microprocessor, actuators); **personal assistants** (e.g. "Vector") using cloud connectivity, voice recognition and computer vision.

**Entertainment** — theme-park character robots, synchronised lighting/laser shows at music festivals, robotic camera control (e.g. the film *Gravity*), humanoid stunt robots using **CGI** and image capture, and precise synchronised special effects.

---

# 6.3 Artificial Intelligence (AI)

## 6.3.1 Introduction

**AI** is the branch of computer science dealing with the **simulation of intelligent human behaviour** — the **cognitive** functions of the brain (acquiring knowledge through thought, experience and the five senses), measured against human benchmarks like reasoning, speech and sight.

## 6.3.2 Characteristics of AI

AI is a collection of **rules and data** with the ability to **reason, learn and adapt** to external stimuli. Three categories:

- **Narrow AI** — superior to a human at **one specific** task.
- **General AI** — **similar** (not superior) to a human at a specific task.
- **Strong AI** — superior to a human at **many** tasks.

**Reasoning** draws conclusions from data; **deductive reasoning** builds correct facts into rules that apply to new problems (e.g. learning to make tea, then applying it to coffee). AI learns, adapts, spots patterns and makes predictions.

**Examples of AI:** news generation; smart home devices (Alexa, Google, Siri, Cortana) recognising voice commands and learning over time; **chatbots**; autonomous cars; facial-expression recognition (mapping landmarks to emotions). *(The **Turing Test** measures a machine's ability to match human intelligence.)*

## 6.3.3 AI systems

Two types covered: **expert systems** and **machine learning**.

### Expert systems

A form of AI that **mimics human knowledge and expertise**, using knowledge and inference to solve problems a human expert would. It gives a conclusion, suggested actions and a **probability** of accuracy.

**Applications:** oil/mineral prospecting, medical diagnosis, fault diagnostics, tax/financial calculations, strategy games (chess), logistics/routing, identifying plants/animals/compounds.

**Structure:**

| Component | Role |
|---|---|
| **User interface** | How the system interacts with the user (dialogue boxes, prompts); questions usually Yes/No, each based on previous answers. |
| **Inference engine** | Main processing part; like a search engine, it matches user input against the knowledge base using the rules base. |
| **Knowledge base** | A **repository of facts** — a collection of **objects** and their **attributes**. |
| **Rules base** | A set of **inference rules** (IF statements) used to draw conclusions. |
| **Explanation system** | Tells the user the **reasoning** behind a conclusion. *(Beyond the core syllabus but included for completeness.)* |

**Setting up:** gather knowledge from experts/sources → populate the knowledge base → create the rules base → build the inference engine → develop the user interface → test with known outcomes.

| Advantages | Disadvantages |
|---|---|
| High expertise, accuracy and consistency; stores vast facts; traceable logic; multiple expertise; very fast; unbiased; gives probabilities. | Users need training; high set-up/maintenance cost; "cold" responses unsuitable for some medical cases; only as good as the data entered; users may wrongly assume it is infallible. |

### Machine learning

A **sub-set of AI** where algorithms are **trained and learn from past experiences/examples**, then make predictions or decisions on **new, unseen data** without being specifically programmed for it. Key strength: managing and analysing large, complex data.

| AI | Machine learning |
|---|---|
| Simulated intelligence; aims to build machines that **think like humans**. | Practice of getting machines to **decide without being programmed to**; learns from data to solve new problems. |

**Examples:**
- **Spam detection** — collect email data, "clean" it (remove stop words/punctuation), flag spam words, train a model on known spam, test live.
- **Buying history** (e.g. Amazon recommendations) — **collaborative filtering** compares customers with similar shopping behaviour to suggest products.
- **Fraud detection** — gather data (survey/**web scraping**), remove redundant data, train on real purchasing behaviour, build and test a model.

**Machine-learning model development:** data collection → data cleaning → exploration & analysis → building a model → model evaluation.

> **Extension — Deep learning:** a sub-set of machine learning that structures algorithms in **layers** (input, hidden, output) as an **artificial neural network** of "nodes", based on the human brain. Excellent at complex visual tasks (e.g. face/bird recognition by analysing pixel values). Needs **large data and high computing power**; its reasoning can be hard to explain (a **"black box"**), unlike machine learning which has clearer rules.

---

# Key terms (quick glossary)

| Term | Meaning |
|---|---|
| **Automated system** | Software + hardware working automatically without human intervention. |
| **Distributed Control System (DCS)** | A powerful computer that monitors and controls a complex process without human interaction. |
| **Adaptive cruise control** | Sensors/actuators/microprocessor keeping a vehicle a safe distance behind another. |
| **Accelerometer** | Sensor measuring acceleration/deceleration and orientation. |
| **Robotics** | Branch of science covering design, construction and operation of robots. |
| **Robot** | A mechanical device that carries out tasks normally done by humans. |
| **Autonomous** | Able to operate independently with no human input. |
| **Controller** | A microprocessor in control of a process (a robot's "brain"). |
| **WebCrawler / search bot** | Software robot that scans and categorises websites. |
| **Chatbot** | A website pop-up robot that appears to converse with users. |
| **End-effector** | An attachment on a robot arm for a specific task (e.g. spraying). |
| **LiDaR** | Light Detection and Ranging; lasers building a 3D image of surroundings. |
| **Drone** | A flying robot (autonomous or remote) used for reconnaissance/deliveries. |
| **Phenotyping** | Observing a plant's physical characteristics to assess health and growth. |
| **Cognitive** | Relating to the mental processes of acquiring knowledge and understanding. |
| **Artificial Intelligence (AI)** | Rules and data giving a system the ability to reason, learn and adapt. |
| **Expert system** | A form of AI that mimics human knowledge and expertise. |
| **Explanation system** | Part of an expert system that explains the reasoning behind its conclusions. |
| **Inference engine** | The processing part of an expert system that matches data to the knowledge base. |
| **Inference rules** | IF-statement rules used by the inference engine to draw conclusions. |
| **Knowledge base** | A repository of facts — a collection of objects and attributes. |
| **Object** | An item stored in the knowledge base. |
| **Attribute** | Something that defines an object in the knowledge base. |
| **Rules base** | A collection of inference rules used to draw conclusions. |
| **Machine learning** | A sub-set of AI in which algorithms are trained and learn from past examples. |
| **Web scraping** | A method of obtaining data from websites. |
| **Deep learning** | A sub-set of machine learning using layered artificial neural networks. |

---

# Quick check questions

1. Describe the roles of sensors, the microprocessor and actuators in an automated system.
2. Give three general advantages and three disadvantages of automated systems.
3. List the six sensors used in an automated weather station and what each measures.
4. Explain how adaptive cruise control keeps a car a safe distance behind another.
5. State Asimov's three laws of robotics.
6. Give the three characteristics a device must have to be called a robot.
7. Explain the difference between an independent and a dependent robot.
8. Describe how an autonomous car senses its surroundings and takes action.
9. Define narrow, general and strong AI.
10. Name the four main parts of an expert system and describe each.
11. Give two advantages and two disadvantages of an expert system.
12. Explain the difference between AI and machine learning, with an example of machine learning.
