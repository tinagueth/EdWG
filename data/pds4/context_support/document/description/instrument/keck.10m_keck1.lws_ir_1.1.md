Instrument Overview
===================
  The long-wavelength spectrometer (LWS) is a mid-infrared imaging
  spectrometer that operates at the Keck I telescope of the W. M.
  Keck Observatory.  The instrument operates with the f/25 secondary
  mirror and is mounted at the forward Cassegrain focus of the
  telescope. It features a Boeing 128 x 128 pixel Si:AS BIB array,
  imaging within a 10.2 x 10.2 arcsecond field, and spectroscopy at
  R=100 or 1400 over the 3-25 micron range.  Chopping and chop-nod
  operating modes are available.  More information on the LWS is
  provided in the paper by Jones and Puetter, 1993
  [JONES&PUETTER1993], and at the web site for the LWS instrument:

    http://www2.keck.hawaii.edu/inst/lws/lws.html


Instrument Characteristics
==========================
  The physical and optical characteristics and estimated imaging and
  spectroscopic performance of the LWS  are provided below. These
  properties are reproduced from the Keck Telescope and Facility
  Instrument Guide, available at
  http://www2.keck.hawaii.edu/observing/kecktelgde/ktelinstupdate.pd
  f. This guide is included as documentation for this archive, by
  permission of the Keck facilities management.


  Physical and optical characteristics
  ------------------------------------
    Dewar hold time      : ~24 hours for LHe, >30 hours for LN
    Guiding system       : One visible-wavelength offset guider
    Scale at detector    : 0.0011 arcsec/micron or
                           0.080 arcsec/pixel
    Detector type        : Boeing Si:As moderate-flux array
    Detector format      : 128 x 128 pixels
    Pixel size           : 75 microns
    Data format          : Six-dimensional FITS file
                           [X,Y,chopbeams,chopsets,nodbeams,nodsets]
                           See below, under 'Data Acquisition'
    Apertures            : 2 longslits, occulting disk, and 'clear'
                           for imaging
    Dispersive elements  : 1 low- and 1 moderate-resolution grating
    Filters              : 14 filters provided
    Collim. focal length : 324 mm
    Camera focal length  : 230 mm
    Pupil size           : 13 mm


    Estimated Imaging Performance
    -----------------------------
      Field of view          : 10.24 x 10.24 arcsec
      Detector pixel scale   : 0.080 arcsec/pixel (75-micron pixel)
      Wavelength range       : 3.5-25 microns
      Standard filters       : Name     Bandpass in microns
                               L        3.5-4.2
                               M        4.4-5.0
                               8.0      7.5-8.2
                               8.9      8.4-9.2
                               9.9      9.4-10.4
                               10.7     10.0-11.4
                               11.7     11.2-12.2
                               12.5     12.0-13.0
                               17.65    17.3-18.2
                               17.9     16.9-18.9
                               18.75    18.3-19.2
                               SiC      10.5-12.9
                               Spec 10  >6.94 (long pass)
                               Spec 20  >13.71 (long pass)
      Image size, 10 micron : 0.25 arcsec FWHM (instantaneous)
                            0.30-0.35 arcsec FWHM (longer exposures)
      Expected count rate   : 11,000 ADU/Jy sec from sky with 11.7
                              micron filter
      Sensitivity to faint  : 17 mJy at 11.75 micron with SiC filter
        stellar objects       100 mJy at 17.65 micron with 17.65
                              filter


  Estimated Spectroscopic Performance
  -----------------------------------
    Total slit length         : 10.24 arcsec
    Usable slit length        : 7.0 arcsec
    Detector scale            : 0.080 arcsec/pixel (75-micron pixel)
    Wavelength range          : 3.5-25 micron
    Order blocking filters    : Name      Bandpass in microns
                                N wide    8.1-13.0
                                Spec 20   >13.71 (long pass)
    Slit widths               : 3, 6 and 12 pixels wide
    Current gratings          : 8 g/mm (10.0 micron blaze); R=100
                                50 g/mm (19.5 micron blaze); R=1400
    Number of grating slots   : 2 slots available, both used
    Corresponding dispersions : LRES: 0.037 micron/pixel
                             HRES: 0.0024 micron/pix (10 micron,N=2)
                             HRES: 0.0048 micron/pix (20 micron,N=1)
    Spectral coverage,        : LRES: 4.7 micron
      single exposure           HRES at 10.0 micron: 0.31 micron
                                HRES at 20.0 micron: 0.62 micron
   FWHM resolution              R=100 and R=1400 (3 pixel slit)
   Count rate at 10micron     : TBD
   Sensitivity to faint       : 150 mJy
     stellar objects


Operational Mode
================
  Chop-nod is the standard mode of data acquisition for the LWS.
  Chopping or tilting of the secondary mirror is performed to cancel
  sky radiation and nodding of the telescope is performed to cancel
  the radiation contribution from the telescope.  The chop-nod
  method for the LWS uses nod and chop throws of equal amplitudes
  but in opposite directions. The result is that for each nod
  position, one of the chop beams is in the same x-y location on the
  detector. The resulting image, after applying a double difference
  process, requires no further shift or add processing.

Data Acquisition
================
  The data acquisition system for the LWS allows the user to choose
  the save-to-disk frequency (maximum 5 Hz) and the total
  integration time. The save frequency and the integration time
  determine the number of chop sets, also called save sets, and the
  number of nod sets. These sets are saved as six-dimensional FITS
  files:

      FITS
      NAXIS  Definition
      -----  -------------------------------------------------------
        1    The number of image columns (X)
        2    The number of image rows (Y)
        3    The number of chop beams
        4    The number of chop frame pairs saved per nod
        5    The number of nod beams
        6    The number of final chop-nod sets

  An illustration of the timing of data acquisition and the ordering
  of chop-nod frames within a six-dimensional FITS file is provided
  in the DOCUMENT/LWS_FITS.JPG file.

  Software
  --------
    Before reducing LWS data, the six dimensions of a raw FITS image
    must be properly combined into a co-added, chop-nod, two-
    dimensional image.  Software to aid this process is available
    from the Keck website for the Infrared Reduction and Analysis
    Facility (IRAF) or for the Interactive Data Language (IDL):

       http://www2.keck.hawaii.edu/inst/lws/wmkolws.html (IRAF)
       http://www2.keck.hawaii.edu/inst/lws/lws-idl.html (IDL)

    Once an image is converted to a two-dimensional array, standard
    optical or infrared processing packages can be used for further
    reductions.