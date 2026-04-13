# SkinnerPudritzCloutier2026-MR-curves
Mass-Radius Curves from Skinner, Pudritz, & Cloutier (2026, revision submitted to MNRAS) as well as validation planet profiles.<br/>
Formatting:<br/>
File Structure: Each folder separates out groups of files, where in each folder only one free compositional parameter is varied (this mostly corresponds to each folder being graphs for a file in the paper). Within each folder, there are different sub-folders for each equilibrium teperature. Within each sub-folder are the files, with names formatted many_radii_WX_Y_Z.txt, where W is the value of the varied compositional parameter, X is the name of the varied compositional parameter, Y is the value of the parameters for the rest of the composition (generally Earthlike), and Z is the temperature. If Z is omitted, it has Earth's temperature. In addition, one folder contains all the validation profiles. This folder contains sub-folders for each object in the validation sample, with their titles reflecting any changes made from the fiducial case. There are two folders for each case: one integrating inwards to the fitting mass, one integrating ouwards to the fitting mass. The full planet profile is the concatenation of the two of them, although note that each thread includes the fitting mass and thus plots may look strange if one of the two datapoints at the same mass is not removed.<br/>
Info (M-R Curves):<br/>
The columns are as follows:<br/>
mass - Mass of the planet (Earth radii)<br/>
envelope_frac - Envelope mass fraction of the planet<br/>
water_frac - Water mass fraction of the planet<br/>
mantle_frac - Mantle mass fraction of the planet<br/>
core_frac - Core mass fraction of the planet<br/>
H_frac_envelope - H fraction of the envelope, by mass<br/>
He_frac_envelope - He fraction of the envelope, by mass<br/>
MgO_frac_mantle - MgO fraction of the mantle, by number<br/>
SiO2_frac_mantle - SiO2 fraction of the mantle, by number<br/>
FeO_frac_mantle - FeO fraction of the mantle, by number<br/>
Fe_frac_solid_core - Atomic Fe fraction of the solid core, by number<br/>
FeS_frac_solid_core - FeS fraction of the solid core, by number<br/>
FeO_frac_solid_core - FeO fraction of the solid core, by number<br/>
Fe_frac_liquid_core - Atomic Fe fraction of the liquid core, by number<br/>
FeS_frac_liquid_core - FeS fraction of the liquid core, by number<br/>
FeO_frac_liquid_core - FeO fraction of the liquid core, by number<br/>
T_eq - Zero-albedo equilibrium temoerature (if there was no internal luminosity) (K)<br/>
albedo - Bond Albedo<br/>
rotation_period - Rotation period (days)<br/>
age - Age (Gyr)<br/>
atmospheric_Z - Metallicity in atmosphere used to calulate opacity (log 
solar)<br/>
100pa_radius - Radius at a pressure of 100 Pa (Earth radii)<br/>
2000pa_radius - Radius at a pressure of 2000 Pa (Earth radii)<br/>
transit_radius - Radius at an optical depth of 2/3 for a transiting ray of light (Earth radii) (THIS IS PROBABLY THE RADIUS YOU WANT, but read section 2.8)<br/>
twothirdsopt_radius - Radius at an optical depth of 2/3 for a ray of light travelling directly to the center of the planet (Earth radii)
condensed_radius - Layer at which planet is made of condensed matter (Earth radii)<br/>
diff_v_2000pa - (transit_radius-2000pa_radius)/transit_radius\*100<br/>
diff_v_100pa - (transit_radius-100pa_radius)/transit_radius\*100<br/>
inner_pressure - Pressure at center of model planet (GPa)<br/>
inner_temperature - Temperature at center of model planet (K)<br/>
Info (Validation):<br/>
The columns are as follows:<br/>
m[Frac_of_total] - Mass as a fraction of total planetary radius<br/>
r[R_e] - Radius in Earth radii<br/>
P[GPa] - Pressure in Gigapascals<br/>
T[K] - Temperature in Kelvin<br/>
Optical_Depth[unitless] - Optical depth, as measured along a line 
directly going to the planetary core<br/>
density[kg/m3] - Density in kg/m3<br/>
ad_grad[unitless] - Unitless adiabatic gradient, defined as adgrad = P/T\*dT/dP<br/>
opacity[m2/kg] - Opacity in m2/kg<br/>
opacity_density[kg/m3] - The density from Freedman+2014 (if not in atmosphere, just the density). Note this is only present for inward planet profiles, not outward planet profiles.<br/>
MgSiO3_melting[K] - Melting temeprature of mantle<br/>
Fe_melting[K] - Melting temperature of core<br/>
phase[see_doc] - Phase of material, see document under validation<br/>
Please direct all correspondance to skinnb1@mcmaster.ca and cite Skinner, Pudritz, & Cloutier (2026, in rev.) if using this work. Mass-radius curves with any of the listed free parameters varied can be generated upon request.