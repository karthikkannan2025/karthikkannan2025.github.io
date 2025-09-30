---
layout: page
title: Senior Design — Poseidon UAV (Blue Skies)
description: Senior Capstone UAV project for NASA Blue Skies competition — disaster-response multirotor
img: assets/img/3.22.jpg
importance: 1
category: work
related_publications: false
---

<div class="mt-2" style="width:100%; overflow:hidden; border-radius:12px;">
  <img src="/assets/img/3.22.jpg"
       alt="Poseidon UAV prototype in testing"
       class="img-fluid"
       style="width:100%; max-height:340px; object-fit:cover;">
</div>

**Summary**  
For my **Senior Design Capstone project**, I worked on **Poseidon**, a custom UAV designed for **hurricane reconnaissance and disaster response**. This project was developed for the **NASA Gateways to Blue Skies competition**, where our team **TRIDENT** was selected as a finalist and recognized for innovation. Our design combined **computer vision, adaptive control, wireless charging landing gear, and modular construction** to create a drone capable of supporting search and rescue missions after hurricanes.  

I served as **Manufacturing Lead** and **Payload/Avionics Lead**, responsible for integrating avionics, designing electrical systems, and supporting structural builds.  

---

### Journey so far
- **2023–2024** — Designed Poseidon UAV for NASA Blue Skies competition.  
- Developed a hurricane-response CONOPS and conducted CAD, FEA, avionics, and propulsion trade studies.  
- Built and flight-tested a working prototype.  
- Submitted and published an [AIAA paper](https://arc.aiaa.org/doi/10.2514/6.2024-85684) on the design.  

---

### Poseidon Features
- **Weight limit:** &lt;10 lbs per NASA rules.  
- **Rotor system:** Hexacopter layout with custom carbon-fiber arms.  
- **Payload:** Cameras, sensors, wireless charging pads, modular avionics bay.  
- **Avionics:** Pixhawk + Raspberry Pi integrated with GPS, IMU, barometers, and telemetry.  
- **Unique:** Wireless charging landing gear + computer vision (YOLOv8).  
- **Mission profile:** Search & rescue, infrastructure inspection, and disaster data collection.  

---

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid
       path="assets/img/SDconops.png"
       title="Poseidon CONOPS Diagram"
       class="img-fluid rounded z-depth-1"
       zoomable=true %}
  </div>
</div>
<div class="caption">
  Concept of operations showing Poseidon mission flow during hurricane response.
</div>

---

### My Role in TRIDENT
I acted as the **OPERATIONS Project Manager**, **Manufacturing Lead** and **Payload/Avionics Lead**, overseeing integration of avionics, payload systems, and electrical components. I also collaborated on structures and manufacturing to ensure subsystem compatibility.  

**Key Contributions**  
- Built and tested the **avionics "nervous system"**, integrating Pixhawk, ESCs, PDB, GPS, and telemetry.  
- Designed and soldered the **Power Distribution Board (PDB)** for modular connections.  
- Helped design **custom landing gear with wireless charging integration**.  
- Assisted with **structural assembly** using carbon fiber and 3D printed parts.  
- Supported testing, data logging, and failure recovery during flight trials.  
- Contributed to the [AIAA publication](https://arc.aiaa.org/doi/10.2514/6.2024-85684).  

---

### Gallery
<div class="row">
  <div class="col-sm mt-3 mt-md-0 text-center">
    <img src="/assets/img/Poseidon_UAV_ISO.png"
         alt="CAD Model of Poseidon UAV"
         class="img-fluid rounded z-depth-1"
         data-zoomable
         style="max-height:250px; object-fit:contain;">
    <p class="mt-2">CAD Model of Poseidon UAV</p>
  </div>
  <div class="col-sm mt-3 mt-md-0 text-center">
    <img src="/assets/img/assembled.png"
         alt="Assembled Nervous System"
         class="img-fluid rounded z-depth-1"
         data-zoomable
         style="max-height:250px; object-fit:contain;">
    <p class="mt-2">Avionics nervous system assembled</p>
  </div>
  <div class="col-sm mt-3 mt-md-0 text-center">
    <img src="/assets/img/IMG_0072.jpg"
         alt="Completed Poseidon Drone"
         class="img-fluid rounded z-depth-1"
         data-zoomable
         style="max-height:250px; object-fit:contain;">
    <p class="mt-2">Completed Poseidon Drone</p>
  </div>
</div>

---

<section class="mt-4">
  <h3>Flight Testing & Lessons Learned</h3>
  <p>
    Testing Poseidon was one of the most exciting and humbling parts of this project. 
    We went through multiple flight trials — some successful, and some that ended with 
    us searching the woods for wreckage.
  </p>

  <h4>Test Flight 1 — March 22</h4>
  <p>
    Poseidon’s first flights revealed weaknesses in our design. On the first attempt, 
    the UAV lifted off but landed hard, snapping the long 3D-printed landing gear. 
    For the second flight, we improvised with pool noodles as landing supports. 
    Poseidon climbed to nearly 200 ft, but due to a <strong>fried GPS unit</strong> 
    (caused by a teammate error), we had to rely only on the Pixhawk as a locator. 
    The UAV drifted toward the treeline, lost connection, and crashed into the forest. 
    We eventually found it with significant damage.
  </p>

  <div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
      <img src="/assets/img/3.22.jpg"
           alt="Poseidon Test Flight 1"
           class="img-fluid rounded z-depth-1"
           data-zoomable
           style="max-height:300px; object-fit:contain;">
      <p class="mt-2">Test Flight 1 — Initial lift-off</p>
    </div>
    <div class="col-sm mt-3 mt-md-0 text-center">
      <img src="/assets/img/FlightTest1.png"
           alt="Poseidon recovered after crash"
           class="img-fluid rounded z-depth-1"
           data-zoomable
           style="max-height:300px; object-fit:contain;">
      <p class="mt-2">Recovered Poseidon after crash</p>
    </div>
  </div>

  <h4>Test Flight 2 — April 13</h4>
  <p>
    After rebuilding Poseidon with redesigned landing gear (shorter supports + pool noodles), 
    we attempted another test. This time, Poseidon lifted off and landed without 
    catastrophic damage. However, yaw and roll instability persisted, and the UAV 
    drifted into the grass. While stability remained an issue, this iteration 
    proved the design was flight-capable and could be tuned with more time.
  </p>

  <div class="row justify-content-sm-center mt-4">
    <div class="col-sm-10 text-center">
      <img src="/assets/img/flying.png"
           alt="Poseidon flying during Test 2"
           class="img-fluid rounded z-depth-1"
           data-zoomable
           style="max-height:400px; object-fit:contain;">
      <p class="mt-2">Poseidon flying during second test</p>
    </div>
  </div>

  <h4>Reflection</h4>
  <p>
    Crashing into the woods may not have been part of our mission plan, 
    but it was a defining moment in our Senior Design journey. The process 
    of debugging hardware failures, improvising solutions, and recovering 
    from setbacks gave us as much practical knowledge as the design work itself. 
    Poseidon ultimately validated its design concepts, laying the foundation 
    for more stable and autonomous future iterations.
  </p>
  <p>
    Because of this project, I became one of the department’s main references 
    for <strong>integrating computer vision into aerospace systems</strong>, 
    supporting other teams and students exploring autonomy and perception. 
    This project also helped me discover my passion for drones. I loved learning 
    the intricacies of building something from scratch, gaining insight into the 
    design process, applications, and the ingenuity required to bring a concept 
    to life. Beyond the technical side, I learned how to work with people who 
    had different mindsets, and even when I butted heads with teammates, those 
    experiences taught me how to cooperate and collaborate more effectively. 
    All of these lessons shaped a project that I am truly proud of — 
    regardless of the results in competition.
  </p>

</section>
