# JWST
Running ML algorithms on JWST data! 
What Are CEERS and JADES?

These are two of the most important early science programs using JWST. You can think of them as big research campaigns that used JWST to observe parts of the universe in great detail.

1) CEERS – Cosmic Evolution Early Release Science Survey
   * It observes a patch of sky called the Extended Groth Strip, and its goal is to Study the formation and evolution of early galaxies! There are at least 50,000 galaxies in its view, giving new clues about the universe's       youth, from its "preteen" years to young adulthood. How cool is that!
   * Instruments used: Primarily NIRCam, NIRSpec, MIRI (Infrared).
  
2) JADES: JWST Advanced Deep Extragalactic Survey
   * It's goal is to Search for the earliest galaxies, possibly from just 200 million years after the Big Bang.
   * Area of observation: Deep fields in GOODS-South and GOODS-North regions (Great Observatories Origins Deep Survey (GOODS))
   * Instruments: NIRCam and NIRSpec.
  

To Know: FITS Files (Flexible Image Transport System)
* Standard format in astronomy
* Stores images, spectra, or tables.
* Requires special libraries to read: astropy.io.fits, photutils, etc.
* Great if you want raw pixel data or more detail.

To Know: CSV Catalogs
* Easy-to-use spreadsheets, ready for ML in pandas
* Contain one row per object (galaxy, star).
* Columns: object ID, RA/Dec (position), magnitude in different filters, redshift, etc.

    
Context
The CEERS catalog contains flux measurements of celestial objects (stars, galaxies) across different wavelength bands (filters), like:

    F435W → ~0.43 µm (blue)
    F606W → ~0.60 µm (visible-red)
    F814W → ~0.80 µm (near-infrared)
These filters simulate how bright an object is at specific wavelengths — kind of like colored sunglasses.
   
WHY???
Stars and galaxies tend to emit light across many wavelengths in predictable patterns (like blackbody radiation or galaxy SEDs). This means:
Fluxes across filters are correlated — and that’s perfect for regression models.

    

   



    

   

    








A tiny note on Groth Strip, because why not? 
The Groth Strip is an image of a small region between the constellations of Ursa Major and Boötes, based on the results of a series of observations by the Hubble Space Telescope. It covers an area 70 arcminutes across and 10 arcminutes wide, which correlates to a patch of sky roughly the width of a finger stretched at arm's length. COOL! 
