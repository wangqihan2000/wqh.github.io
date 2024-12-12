---
title: "Investigation of Duality between EKF and Receding Horizon Estimator"
excerpt: "This paper investigates the duality between two prominent estimation techniques—Extended Kalman Filter (EKF) and Receding Horizon Estimator (RHE)—in the context of spacecraft navigation. <br/><img src='/images/dock.PNG'>"
collection: portfolio
---

* <b>Tech Stack:</b> Julia, Python, Control Theory

* <p style="text-align: justify;"><b>Introduction</b><br>This paper investigates the duality between two prominent estimation techniques—Extended Kalman Filter (EKF) and Receding Horizon Estimator (RHE)—in the context of spacecraft navigation. These methods are employed to handle dynamic systems operating in noisy environments, where delays occur between sensor measurements and their integration into state estimators. The project explores their efficacy for SpaceX Dragon 1’s relative navigation to the International Space Station (ISS). Through mathematical analysis and simulation, the paper aims to compare these techniques to reveal their strengths and limitations in optimizing state estimation and control for dynamic aerospace systems.</p>
  
* <p style="text-align: justify;"><b>Method</b><br>The research focuses on assessing the performance of EKF and RHE under conditions of variable measurement delays and noise. EKF, a recursive Bayesian filter, estimates the state of nonlinear systems by linearizing system dynamics around current estimates of state and covariance. Meanwhile, RHE operates within the Model Predictive Control (MPC) framework, continuously updating state estimates based on the latest available measurements, by solving an optimization problem over a finite time horizon. This enables RHE to adaptively refine trajectory predictions and control inputs for spacecraft navigation. Both techniques are tested using full state and range-bearing measurements to ensure accurate navigation in noisy conditions.</p>

    <div style="text-align:center">
    <img src="/images/MPC.PNG" alt="buggy_lqr_plots" style="width:400px;height:230px;">
    </div>
    
    <img src="/images/EKF_RHE.PNG" alt="buggy_lqr_plots" style="width:350px;height:400px;">
    </div>
    
* <p style="text-align: justify;"><b>Results</b><br>The paper presents simulation results that compare the trajectory accuracy of EKF and RHE. The EKF approach, which relies on linearizing system dynamics, shows higher accuracy but introduces more noise sensitivity. RHE, on the other hand, yields a smoother trajectory due to its real-time optimization over a horizon, although it is computationally more intensive. The results highlight that while EKF is faster and more accurate in some scenarios, RHE offers better trajectory smoothness and robustness in handling measurement noise. Root Mean Square Error (RMSE) values show EKF having lower error than RHE, but RHE offers better noise compensation.</p>

    <div style="text-align:center">
    <img src="/images/traj.PNG" alt="buggy_lqr_plots" style="width:690px;height:600px;">
    </div>

* <p style="text-align: justify;"><b>Conclusion</b><br>The study reveals that both EKF and RHE have their own advantages. EKF’s recursive structure allows for quick updates with less computational burden, but it is more sensitive to noise. RHE, being part of the MPC framework, provides better noise handling and trajectory smoothness but at the cost of higher computational requirements. The duality between the two methods suggests they can be complementary, depending on mission needs. Future work could focus on enhancing RHE’s computational efficiency and exploring its application in more complex systems like multi-legged robots.</p>
