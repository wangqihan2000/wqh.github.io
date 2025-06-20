---
title: "Automated Grasp Point Generation for Wire Grippers in Binder-Jet Metal Additive Manufacturing"
excerpt: " This research presents a novel algorithm for generating grasp point candidates on any 3D objects using wire grippers <br/><img src='https://wangqihan2000.github.io/wqh.github.io/images/setup.png'>"
collection: portfolio
---

* <b>Tech Stack:</b> Python, PointClouds, ROS, Docker, Nvidia ISAAC Sim, RViz, Arduino, SW, Machining/Manufacturing

* <p style="text-align: justify;"><b>Abstract</b><br>De-powdering is a critical step in binder jet metal additive manufacturing, which requires efficient and automated solutions to remove residual powder while maintaining part integrity. This research presents a novel algorithm for generating grasp point candidates on any 3D objects using wire grippers wires bent in certain directions. The method involves projecting STL models onto a 2D bitmap to extract a silhouette, applying morphological dilation and contour detection to identify key boundary features, and classifying grasp points based on curvature analysis. A direction-aware selection processdetermines four optimal grasping points with corresponding orientations, ensuring stable lifting configurations. The grasping strategy is further validated in NVIDIA Isaac Sim through physics based simulations, where wire grippers attempt to lift and stabilize parts. The results demonstrate the robustness of the proposed approach in identifying reliable grasp points for diverse 3D geometries, paving the way for automated depowdering solutions in industrial additive manufacturing workflows. The progress in the solution establishes binder jet metal 3D printing as a cutting-edge method for producing complex, high-performance parts with diverse industrial applications. This research drives additive manufacturing forward by opening up new opportunities for scalable and flexible production systems in contemporary industry.</p>

Here is the [Article link](/wqh.github.io/files/Final_paper.pdf)!
