Mardlamock-DeathRocket
======================

This is in response to https://www.reddit.com/r/rocketry/comments/27xm6s/should_i_launch/

#Analysis

The motor pressure is flirting with the burst presure of the casing, it will probably explode.

If somehow it does not CATO, the rocket is so overpowered that the airframe has no chance of surviving flight at nearly Mach 3.

The rocket is surprisingly stable, but mainly because there is an unreasonable amount of fuel extending forward of the CoG.

The only possible chance of survival is that OP's fuelmaking technique is so different from anyone elses that he ends up with a slow burning, low exponent, version of KNSU. This would be exciting but I consider it unlikely.

**Bottom Line: No you should not launch this.**

There is just too much fuel for the motor, and too much motor for the rocket.


##Motor
<!--Begin motor DeathMotor HTML export from MotorSim-->
<table class='motor' style='text-align: left; border: 1px solid black'><tr><th colspan='6' class='title'>DeathMotor</th></tr><tr class='summary'><th>Rating:</th><td>8% K-1092</td><th>Max Pressure:</th><td>7.96 MPa</td></tr><tr class='summary'><th>Total Impulse:</th><td>1362 Ns</td><th>Specific Impulse:</th><td>137 s</td></tr><tr class='summary'><th>Max Thrust:</th><td>1445 N</td><th>Volume Loading:</th><td>84%</td></tr><tr class='summary'><th>Average Thrust:</th><td>1092 N</td><th>Fuel Mass:</th><td>1016 g</td></tr><tr><td colspan='4' class='thrust'><img src='http://chart.apis.google.com/chart?chxt=x,x,y,y,r,r&chs=400x200&cht=lxy&chco=3072F3&chds=0,1.25,0,1445.11&chxr=0,0,1.25|2,0,1445.11|4,0,324.87&chd=t:0,0,0,0,0,0,0,0,0,0,0.01,0.03,0.06,0.11,0.19,0.31,0.49,0.78,0.91,1.1,1.11,1.24,1.25|0,49.09,93,304.57,332.38,358.44,382.87,405.75,427.21,447.32,710.09,750.56,788.6,848.57,941.31,1078.29,1259.09,1425.55,1445.11,1405.08,724.13,0.39,0.32&chxl=1:|s|3:|N|5:|lbf&chxp=1,50|3,50|5,50' width='400' height='200' alt='null' /></td></tr></table>
<!--End motor DeathMotor-->

With a burn time of just over one second and a max pressure of 8Mpa or 1,100psi this motor has a safty margin of about zero. With pressure so close to burst estimates for sch40 PVC there is a high likelyhood of CATO.

KNSU exhibits higher burn rates at higher pressures, which leads to higher pressure still. For this reason the motor calculations are highly influenced by the burn rate exponent which needs to be measured. Reported caramelization might lead to lower burn rates, longer burn time, and lower pressure.

If Mardlamock were to perform a static test, **taking serious precautions against the likelyhood of failure** and measure the burn time we could fudge the burn rate exponent until the calculations match the burn time.

##Flight

###Stability

I had assumed the rocket would be understable from looking at the picture. However, the fuel makes up more than half of the total launch mass, and it extends so far forward in the rocket that it pushes the CoG *forward*. I am used to shorter motors, compared to the length of the airframe. Stability at launch, 2.66 cal, 2 cal at burnout.

**May be overstable at launch, creating undesired weathercocking if there is wind.**

###Speed

OpenRocket simulates a max velocity of 954m/s or 2114mph or **2.7 Mach**

**NO Just no**. The fins will come off, the nose cone will fail, anything that does not come off will catch fire.

Acceleration is brutal, 100G+

###Altitude

About 3km. Accelleration is brutal, but empty rocket is so light and going so fast that deceleration is brutal too. 

#Assumptions

##Motor

* Chamber
	* Inner chamber length: 2cm
		* **This can't be right? Guessing 43cm**
	* Inner chamber diam: 4.34cm
* Nozzle
	* **I am assuming these were switched in the reddit post** 
	* Nozzle throat diam: 1.25cm
	* Nozzle exit diam: 4.34cm
* Motor casing
	* **Assuming 2 inch schedule 40** 
	* 5cm diam, 32mm thick white pvc.
		* **I think these are wrong, no PVC is that thick**
		* **Assuming***
		* 5cm OD
		* 4.34cm ID
		* 3.2mm Thickness
		* 4.34cm + .64mm = 5cm 
* Motor length overall: 65cm,
* Motor empty weight 550g approx

##Fuel

* Sugar is regular tabletop sugar
* 1 KG Fuel
	* 350g of it for real rocket
		* **This must be just the sugar** 
	* Assuming 650g KN 
* o/f ratio is 65:35
* Fuel density: 0.302g/cm3,
* Fuel grain geometry
	* regular bates grain
	* **How Many? Guessing 4 from size & weight**
	* **Outer Diameter? Guessing 4.34cm**
	* Each 10cm long and with a 
	* 1cm diam empty cilinder in the middle.

##Airframe

* Fin
	* shape: triangular
	* 5cm base
	* 15cm height
	* 0.4cm thick 
	* Material: wood (unknown)
* Nosecone
	* Shape: conical
	* Material: fiberglass
	* Weight: I'd say around 30g approx
* Total mass is is 1.65kg, no idea where cog is.
	* **This needs to be measured**
	
I have performed several static tests and 2 thrust measurements, burn time of the real rocket is 10seconds, max thrust 10kgf, average 6, 5-7, 5. I am doing another one tomorrow with 300g of fuel, to see a bit better how it behaves
