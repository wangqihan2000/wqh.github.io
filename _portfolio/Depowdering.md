---
title: "Automated Grasp Point Generation for Wire Grippers in Binder-Jet Metal Additive Manufacturing"
excerpt: " This research presents a novel algorithm for generating grasp point candidates on any 3D objects using wire grippers <br/><img src='https://wangqihan2000.github.io/wqh.github.io/images/setup.png'>"
collection: portfolio
---

* <b>Tech Stack:</b> Python, PointClouds, ROS, Docker, Nvidia ISAAC Sim, RViz, Arduino, SW, Machining/Manufacturing

* <p style="text-align: justify;"><b>Abstract</b><br>De-powdering is a critical step in binder jet
 metal additive manufacturing, which requires efficient
 and automated solutions to remove residual powder
 while maintaining part integrity. This research presents
 a novel algorithm for generating grasp point candidates
 on any 3D objects using wire grippers wires bent in
 certain directions. The method involves projecting STL
 models onto a 2D bitmap to extract a silhouette, applying
 morphological dilation and contour detection to identify
 key boundary features, and classifying grasp points based
 on curvature analysis. A direction-aware selection process
 determines four optimal grasping points with correspond
ing orientations, ensuring stable lifting configurations.
 The grasping strategy is further validated in NVIDIA
 Isaac Sim through physics-based simulations, where wire
 grippers attempt to lift and stabilize parts. The results
 demonstrate the robustness of the proposed approach
 in identifying reliable grasp points for diverse 3D ge
ometries, paving the way for automated depowdering
 solutions in industrial additive manufacturing workflows.
 The progress in the solution establishes binder jet metal
 3D printing as a cutting-edge method for producing
 complex, high-performance parts with diverse industrial
 applications. This research drives additive manufacturing
 forward by opening up new opportunities for scalable and
 flexible production systems in contemporary industry.</p>
  
* <p style="text-align: justify;"><b>Method</b><br>The research focuses on assessing the performance of EKF and RHE under conditions of variable measurement delays and noise. EKF, a recursive Bayesian filter, estimates the state of nonlinear systems by linearizing system dynamics around current estimates of state and covariance. Meanwhile, RHE operates within the Model Predictive Control (MPC) framework, continuously updating state estimates based on the latest available measurements, by solving an optimization problem over a finite time horizon. This enables RHE to adaptively refine trajectory predictions and control inputs for spacecraft navigation. Both techniques are tested using full state and range-bearing measurements to ensure accurate navigation in noisy conditions.</p>

    <div style="text-align:center">
    <img src="https://wangqihan2000.github.io/wqh.github.io/images/MPC.PNG" alt="buggy_lqr_plots" style="width:400px;height:230px;">
    </div>
    
    <img src="https://wangqihan2000.github.io/wqh.github.io/images/EKF_RHE.PNG" alt="buggy_lqr_plots" style="width:350px;height:400px;">
    </div>
    
* <p style="text-align: justify;"><b>Results</b><br>The paper presents simulation results that compare the trajectory accuracy of EKF and RHE. The EKF approach, which relies on linearizing system dynamics, shows higher accuracy but introduces more noise sensitivity. RHE, on the other hand, yields a smoother trajectory due to its real-time optimization over a horizon, although it is computationally more intensive. The results highlight that while EKF is faster and more accurate in some scenarios, RHE offers better trajectory smoothness and robustness in handling measurement noise. Root Mean Square Error (RMSE) values show EKF having lower error than RHE, but RHE offers better noise compensation.</p>

    <div style="text-align:center">
    <img src="https://wangqihan2000.github.io/wqh.github.io/images/traj.PNG" alt="buggy_lqr_plots" style="width:790px;height:690px;">
    </div>

* <p style="text-align: justify;"><b>Conclusion</b><br>The study reveals that both EKF and RHE have their own advantages. EKF’s recursive structure allows for quick updates with less computational burden, but it is more sensitive to noise. RHE, being part of the MPC framework, provides better noise handling and trajectory smoothness but at the cost of higher computational requirements. The duality between the two methods suggests they can be complementary, depending on mission needs. Future work could focus on enhancing RHE’s computational efficiency and exploring its application in more complex systems like multi-legged robots.</p>
