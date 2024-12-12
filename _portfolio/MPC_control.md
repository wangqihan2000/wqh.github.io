---
title: "Multi Control theories used to simulate the vehicle path"
excerpt: "Implemented various control techniques on a Tesla simulation. <br/><img src='/images/control_page.PNG'>"
collection: portfolio
---

* <b>Tech Stack:</b> Python, Webots

*  <p style="text-align: justify;"><b>Introduction</b><br>This project focuses on designing and implementing control systems for lateral vehicle dynamics using a state-space model. The tasks include checking the controllability and stabilizability of a linearized system, designing a lateral full-state feedback controller, and evaluating its performance in Webots simulation software. The project aims to achieve robust lateral control for an autonomous vehicle, ensuring stability and accuracy in trajectory tracking under various dynamic conditions.</p>
  
* <p style="text-align: justify;"><b>Method</b><br>The model considers error-based linearized state-space representations of the lateral dynamics of a vehicle. Controllability and stabilizability are evaluated for longitudinal velocities ranging from 1 m/s to 40 m/s. For control design, a state feedback controller with pole placement is developed to meet specific performance criteria. Python-based simulations in Webots are used to test the designed controllers, utilizing tools like SciPy for pole placement and matrix computations. System performance is analyzed through trajectory tracking and state deviations.</p>

* <b>Results</b>
    * <p style="text-align: justify;"><b>The designed controller is expected to ensure stability and accurate trajectory tracking</b>, with the following performance benchmarks:<br>
      1. Completion of the track in less than 350 seconds.<br>
      2. Maximum deviation from the reference trajectory limited to 9 meters.<br>
      3. Average deviation from the reference trajectory below 4.5 meters.<br><br>
      The project provides insights into how different pole placements influence system response and stability. Performance plots, including state trajectories and pole dynamics, offer a quantitative evaluation of the control system's effectiveness.</p>

    <p>With LQR, the time taken to complete the track was 152.96 s. Which is significantly faster than the PID.</p>

    <div style="text-align:center">
    <img src="/images/LQR.PNG" alt="buggy_lqr_plots" style="width:500px;height:400px;">
    </div>

