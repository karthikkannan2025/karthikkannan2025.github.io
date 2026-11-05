---
layout: page
title: "Tobio — Volleyball Setter Robot"
description: "Trajectory modeling, ESP32 control, and a small-scale launcher prototype"
category: fun
importance: 0
status: "Prototyping"
related_publications: false
---

## Why I am building it

Tobio is my attempt to turn a volleyball set into a repeatable robotics problem. The goal is a machine that can deliver different types of sets by controlling where the ball goes and how long it takes to get there. It gives me a concrete reason to learn the mechanics, electronics, and control software needed to make a physical system behave predictably.

I am starting with a **ping-pong-ball prototype** before scaling to volleyball hardware. That lets me work through launcher geometry, motor control, and wiring on a smaller system. It is a development platform; a full-size volleyball machine remains the goal.

## From a target to a launch command

The Python trajectory code starts with a launcher position, a target position, and a requested **time of flight**. It solves for the initial velocity vector, then converts that into launch speed, pitch, and yaw. Keeping time of flight explicit matters because two balls can arrive at the same place with very different trajectories and timing.

I keep that math separate from hardware control. Set presets can be reused by the simulation tools and the controller, while changes to motor hardware do not require rewriting the trajectory model. The current model is a **drag-free approximation**, useful as a starting point rather than a claim of measured accuracy.

## Connecting the model to hardware

The ESP32 firmware estimates wheel RPM from launch speed and translates that estimate into **open-loop PWM** for two BTS7960 motor drivers. It includes serial commands for set presets and explicit arm, stop, and disarm states. The current build planning uses two 775 motors, a Raspberry Pi/ESP32 setup, and pitch/yaw servos with a separate regulated power supply.

The electrical work has been a project of its own: separating logic and motor power, planning fuses and a contactor, and incorporating an emergency stop and driver-enable interlock. Recent work has focused on parts, assembly, and resolving the practical connections between those components.

## The gap between a model and a repeatable set

The next major step is calibration: **PWM → wheel RPM → ball exit speed → landing position**. Wheel contact, slip, and the ball itself affect the result, so initial motor and transfer-efficiency estimates need to be replaced with measurements. A solved trajectory does not yet mean the launcher can reproduce it.

I have trajectory software, firmware, CAD concepts, and an ongoing hardware prototype. Repeatable launches, measured accuracy, and scaling to a volleyball are still ahead. That is the part I am most interested in: using test results to close the gap between what the code predicts and what the machine actually does.

**Tools and focus:** Python, ESP32/Arduino, embedded control, trajectory modeling, CAD, electrical integration, and experimental calibration.
