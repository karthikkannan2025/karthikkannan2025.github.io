---
layout: page
title: REACHR
description: (Currently working on) Autonomous drone designed for FEMA/NASA relief missions
img: assets/img/REACHR_PIC.png
importance: 1
category: work
related_publications: false
---
<div class="mt-2" style="width:100%; overflow:hidden; border-radius:12px;">
  <img src="/assets/img/reachr-hero-banner.png"
       alt="REACHR HERO vehicle hovering during field test"
       class="img-fluid"
       style="width:100%; max-height:340px; object-fit:cover;">
</div>

**Summary**  
REACHR is building **HERO 2**, a VTOL-capable flying boat UAV for disaster response. The system blends high-resolution imaging, IR sensing, real-time data links, and a hybrid-electric powertrain for long-endurance operations in flooded or remote areas. I contribute on autonomy, networking, and electrical integration.

The **REACHR Project** at NC State University is developing **HERO 2**, a VTOL-capable flying boat UAV for disaster response. HERO 2 combines high-resolution imaging, infrared sensors, real-time data transmission, and a hybrid-electric powertrain for long-endurance autonomous operations in flooded or remote areas.  

Our mission is simple: **advance unmanned aerial system technology for critical response and surveillance.** With a multidisciplinary student team, REACHR aims to redefine how UAVs move and operate, ensuring efficient and effective performance when people need it most.  

### Journey so far
- **2023** — Project initiated at NC State to design a disaster-response UAV.  
- **2024** — Won NASA Blue Skies **Most Innovative** award.  
- **2025** — Awarded an **$80K USRC grant** to build a full-scale prototype with FEMA and NCDPS for Ocracoke Island, NC.  

### HERO 2 operations include
- Swift deployment with modular assembly and VTOL take-off.  
- Hybrid-electric climb to altitude for endurance and coverage.  
- Infrared scanning to detect survivors and hazards.  
- Ground-station processing for optimized rescue planning.  
- Network dissemination for real-time coordination with agencies.  
- Rapid refitting with modular payloads for future missions.  

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid
       path="assets/img/reachr_conops.png"
       title="REACHR CONOPS Diagram"
       class="img-fluid rounded z-depth-1"
       zoomable=true %}
    
  </div>
</div>
<div class="caption">
  Concept of operations showing HERO 2 mission flow from launch to rescue support.
</div>

The **REACHR Concept of Operations (CONOPS)** illustrates how HERO 2 supports disaster response missions end to end.  

1. **Rapid Assembly & Launch** — Modular field assembly; VTOL from land or water.  
2. **Climb to Altitude** — Hybrid-electric powertrain for efficient climb and long endurance.  
3. **Heartbeat Detection** — NASA FINDER and IR payloads scan for survivors, hotspots, and hazards.  
4. **Rescue Planning** — Ground-station processing and AI tools generate an optimized rescue plan.  
5. **Network Dissemination** — Plans shared via the REACHR network for real-time coordination.  
6. **Mission Refitting** — Quick reconfiguration for surveillance, delivery, or continued response.  

Together, this cycle delivers critical data quickly, improves situational awareness, and accelerates rescue operations in flooded or isolated regions.  

<div class="row">
  <div class="col-sm mt-3 mt-md-0 text-center">
    <img src="/assets/img/REACHR_Electrical_diagram.png"
         alt="REACHR Electrical Diagram"
         class="img-fluid rounded z-depth-1"
         data-zoomable
         style="height:250px; width:100%; object-fit:contain;">
    <p class="mt-2">Electrical system diagram</p>
  </div>
  <div class="col-sm mt-3 mt-md-0 text-center">
    <img src="/assets/img/REACHR_WING_ANSYS.jpg"
         alt="REACHR Wing ANSYS Simulation"
         class="img-fluid rounded z-depth-1"
         data-zoomable
         style="max-height:250px; object-fit:contain;">
    <p class="mt-2">Wing analysis in ANSYS</p>
  </div>
  <div class="col-sm mt-3 mt-md-0 text-center">
    <img src="/assets/img/PIXHAWK_JETSON.png"
         alt="Pixhawk + Jetson Integration"
         class="img-fluid rounded z-depth-1"
         data-zoomable
         style="max-height:250px; object-fit:contain;">
    <p class="mt-2">Pixhawk + Jetson integration</p>
  </div>
</div>

<div class="caption">
  These are some of the things I have worked on and assisted with.
</div>


<section>
  <h3>My Role in REACHR</h3>
  <p>
    I focus on the <strong>autonomy, networking, and electrical integration</strong> of HERO 2, bridging algorithms, communications, and hardware reliability to ensure the aircraft can operate in demanding conditions.
  </p>
  <p>
    Although I was not part of the initial REACHR senior design team, I joined soon after while leading my own project. Rather than working in isolation, I collaborated with REACHR members by assisting with system tuning, setup, and sharing components such as computer-vision modules. This collaboration has been rewarding, and I believe REACHR demonstrates the real potential of UAVs in humanitarian response and disaster relief.
  </p>

  <h4>Key Contributions</h4>
  <ul>
    <li>Developed and tested <strong>landing algorithms</strong> using computer vision for reliable detection and touchdown.</li>
    <li>Integrated <strong>Starlink connectivity</strong> and configured mobile hotspots to enable real-time data streaming from the UAV.</li>
    <li>Produced and maintained <strong>electrical diagrams</strong> and supported the <strong>internal electrical system layout</strong> for avionics and payloads.</li>
    <li>Established <strong>hardware monitoring</strong> to track power and system health during testing.</li>
    <li>Contributed to <strong>operational documentation and checklists</strong>, linking technical workflows with field procedures.</li>
  </ul>
</section>
