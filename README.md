# DICE_model_extension
 The code in this repository extend the MPC-DICE model code written by Timm Faulwasser, Christopher Kellett and Steven R. Weller (https://www.researchgate.net/publication/325145766_MPC-DICE_An_open-source_Matlab_implementation_of_receding_horizon_solutions_to_DICE).
 In this version of code, based on th research on green bond and DICE model (Orlov, Sergey and Rovenskaya, Elena and Puaschunder, Julia M. and Semmler, Willi, Green Bonds, Transition to a Low-Carbon Economy, and Intergenerational Fairness: Evidence from an Extended DICE Model (December 12, 2017). Available at SSRN: https://ssrn.com/abstract=3086483 or http://dx.doi.org/10.2139/ssrn.3086483)

To incorporate green bond and tax to the model, two key equations are added
<img src="https://github.com/FengheliuDavid/DICE_model_extension/assets/117461483/86437bf5-15bb-4dd3-b604-4e5aeefb1fbe" alt="eq1" width="500" >
<img src="https://github.com/FengheliuDavid/DICE_model_extension/assets/117461483/9747ab27-4782-4829-94b2-bd02337190e4" alt="eq1" width="250" >


Compared to the original model, in this code, in the time period of excess mitigation cost over taxation, mitigation cost are paid via bonds. Also, besides capital stock, green bond stock is add, tax is levied on net GDP

The data is included in the assign_parameters_v2020.m, I get the data of bond rate, discount rate, etc. by literature view, Bloomberg, IMF, Euromonitor, NBER, World Bank, etc.

The code uses casadi to solve the multi-stage optimization
 
