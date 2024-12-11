java c
MECH5900M Assignment 2024 Autumn 
Assignment Guideline 
• Poor visualisation of the results will be penalised. See the bad  good examples on the next page.
• This is an individual assignment. You are not allowed to discuss the assignment with anyone. Do not share or discuss the assignment, results or codes with anyone.
• The total mark of this assignment is 100%, which is 50% of the total module mark.
• The submission link will appear on the Minerva module website.
• The report file format to be submitted is pdf. Use the pdf generation function in MS Word or print it in PDF format. Or use LaTeX.
• In the report, use 11pt font size and single line space. The maximum page is 6 pages excluding the appendix. The report beyond 6 pages will not be marked.
• Include all Matlab m-scripts and Simulink blocks used in the report in the appendix. The appendix is not included in the page limitation.
• Questions for the assignment would be answered only if the questions were to clarify the tasks. The questions about how to do it will not be answered until the report is submitted.
Bad  Good Visualisation Examples 

Figure 1: Bad Example: Screenshot of a scope block (dark background), no units, no labels, too small fonts to read, figure size too small

Figure 2: Good Example: draw the plot using ”plot command”: units, labels, good font size and figure size, legends
In line with the University guidance on the use of generative-AI, all written reports on MECH5900M are categorised as AMBER. The only ways in which Generative-AI is acceptable for these written reports are:
• as a search engine to help you to find sources of information,
• providing ideas or inspiration,
• to summarise or translate source documents to aid reading,
• as a grammar checker.
The University recommended tool is https://copilot.microsoft.com/, where the data you input is private (when logged in through your University IT account) and the original sources of the information are given.
Remember that you are responsible for the content of any reports submitted and any material taken from another source should be clearly acknowledged. Any text which is not in quotation marks must be written by you. 
You should always take a critical approach to the use of any output from a gen-erative AI tool, as these tools can generate superficial, inaccurate and unhelpful outputs.
More guidance is available here:
• https://generative-ai.leeds.ac.uk/ (Including how to acknowledge the use of generative-AI)
• https://generative-ai.leeds.ac.uk/uol-genai-guidance-for-taught-students/ (stu-dent guidance PDF)
• https://students.leeds.ac.uk/info/1000127/artificial-intelligence-ai (student web pages)
Please seek guidance from your module leader if you are unsure about appro-priate use of generative-AI tools.
代 写MECH5900M Assignment 2024 AutumnR
代做程序编程语言Task 1. Active Nutation with Gas Thruster [60%] 
The moment of inertia of a rocket is given by

and the initial angular velocity at time t = 0 is given by

The desired angular velocity is equal to

The rocket is equipped with thrusters for b1 and b2 axes, where the torque is either +0.5, 0.0 or -0.5 Nm for each axis. For b1 and b2 body axes, the linearised dynamics can be written in the following state-space form. as follows:

• Define x and u and obtain the numerical values for A and B for the active nutation damping control and check the stability without any feedback control. [10%]
• The active nutation control is to be designed using the LQR (Linear Quadratic Regulator) control algorithm with the ideal actuator assump-tion providing varying magnitude torques. Determine Q and R in the LQR design to satisfy the following requirements:
– both |ω1| and |ω2| shall converge to the values less than 0.0001 rad/s in less than 50 seconds [10%]
– the magnitude of all the elements of u from the LQR controller shall be always less than 0.5 Nm [10%].
Show the simulation results satisfying the above two requirements using the nonlinear dynamic simulator implemented in Simulink [10%].
• Determine the on and off values of the Schmitt trigger for the LQR de-signed to use the gas thrusters satisfying the following requirements:
– both |ω1| and |ω2| shall converge to the values less than 0.0001 rad/s in less than 50 seconds [10%]
Show the simulation results satisfying the above two requirements using the nonlinear dynamic simulator implemented in Simulink [10%].
Task 2. Robustness Analysis [30%] 
The controller designed in Task 1 with the Schimitt trigger is to be tested for its robustness with respect to the uncertainties in the moment of inertia, J. The true J is now perturbed as follows:

All the other simulation parameters including the LQR and the Schmitt trigger and the initial angular velocities remain the same as ones in Task 1. Let the uncertainty be in the ranges of the following inequalities:
−0.1 ≤δ1≤ 0.1
−0.1 ≤δ2≤ 0.1
−0.05 ≤δ3≤ 0.05
−0.05 ≤δ12≤ 0.05
−0.05 ≤δ13≤ 0.05
−0.05 ≤δ23≤ 0.05
Generate random δ1, δ2, δ3, δ12, δ13 and δ23 uniformly distributed in the inter-vals given in the above and perform. 1000 simulations. From each simulation, calculate the settling time, ts, which is defined by
|ω1(t)| ≤ 0.0001 [rad/s] and |ω2(t)| ≤ 0.0001 [rad/s], for t ≥ ts                                    (6)
and draw the plot ts (the vertical axis in the plot) with respect to ∥δ∥ (the horizontal axis in the plot), where

and

[30%]
Task 3. Limitations  Presentation [10%] 
Explain the limitations of the controller designed and verified in Tasks 1 and 2 to general audiences. [10%]





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
