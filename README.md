Manual for the Program: Shielding Calculation for Radiotherapy Facility 

This general-purpose program calculates workload, shielding attenuation factor, & advised 
wall thickness for the shielding design of a radiotherapy facility. It is in reference to the 
NCRP 151 report.  
There are two programs, one for general purposes that includes a section for secondary 
barriers calculation and one named “example” is only specific to the class project. 
Note: shielding design doesn’t include IMRT contributions. 
Modules: 
• Workload Calculation 
• Shielding Attenuation Factor (B) Calculation 
• TVLs (Tenth-Value Layers) and Barrier Thickness Calculation 
Make sure you have following Inputs: 
• Patient load at your facility, patient treatment frequency, dose per patient. 
• Use factor (U), occupancy factor (T), shielding design goal (P). 
• Distance from the radiation source and material properties. 
Below is a step-by-step guide for using this program. 
1. Setup: Run the program in a Python environment or Jupyter Notebook.
 2. Workload Calculation: The program requires you enter number of patients treated per 
day per week, number of treatment days in a week, dose value and its unit (Gy or mR). If 
the units are mR the program will convert to Gy and use the Gy unit in the calculation. 

3. The program will next present you with tables for P, U, T from NCRP 151 and enter the 
above calculated value for W. 
4. Shielding Attenuation Factor calculation: Enter the permissible value of dose behind 
that barrier from the table given in the program. Enter the above workload, enter the 
value of U & T from the table to get the shielding attenuation factor& number of TVL as 
the output. 

5. The program will next present you with TVL table for wall thickness. 
6. Calculate Wall Thickness: Input the TVL1 and TVLe values. And followed by this, the 
program calculates the required wall thickness. 
Outputs 
• Workload: Weekly dose delivered by the linac (e.g., 450 Gy/week). 
• Shielding Attenuation Factor (B): Fraction of radiation attenuated. 
• Number of TVLs (n): Required for achieving the attenuation. 
• Wall Thickness (t): Total thickness in cm based on the TVL values. 
This is a basic manual to get the program running by anyone. A basic knowledge of 
these terms would be helpful to understand it better. If you need more information 
refer to NCRP 151 .
