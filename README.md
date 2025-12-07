Thank you for checking out my Analytical Mechanics term project! 
If you would like to run the code in ISS_Observation_Path/Simulation, please continue reading. 

I developed a visual simulation of the International Space Station's relative motion using SymPy and MatPlotLib. 
SymPy is a very straightforward library that acts as a functional CAS for replacing numerical computation with symbolic computation.
However, when used with MatPlotLib, not every python IDE handles it the same way. 

I code on my macbook M3 Max using Spyder, which operates between the set os filepaths and its own internal directory. 
If you also use Spyder or any similar IDE, be sure to condirm that its graphics backend is not set to "inline".
In Spyder's console: Tools -> Preferences -> IPython Console -> Graphics -> Backend Dropdown Menu
To allow the simulation window to appear, set this to "automatic" or "Qt" instead of "inline". 

Then just run the file and observe!

If you would like to see what the path of the ISS looks like with respect to your position, find these literals: 

Line 14: phi0_deg = 28.083 
Line 15: lambda0_deg = -80.608

These are the latitude and longitude of the Ortega Observatory, respectively. 
Change them to your position on the globe and rerun the simulation. If the graphs move out of frame, find these ranges:

Line 145: ax_local.set_xlim(-7500,7500)
Line 146: ax_local.set_ylim(-7500,7500)
Line 147: ax_local.set_zlim(-10000, 5000)

These are the X, (East / West) Y, (North / South) and Z (Zenith) axes, respectively. 
Change them to accomodate the rotation of the relative ISS path that occurs due to the change in latitude. 

Enjoy!
