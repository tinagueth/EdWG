
 
      The camera state description was provided by the NAVCAM
      instrument Science Lead, Raymond L. Newburn, Jr., while the rest of
      the description was copied from ``STARDUST Navigation Camera
      Instrument Description Document' with permission from the Stardust
      project.
 
      SDN:  This document has been updated for the Stardust-NExT (SDN)
      mission, but mostly left intact from the prime mission data sets.
      The prefix 'SDN:' typically precedes updated material.
 
 
    Navigation Camera Overview
    ==========================
 
      The NAVCAM, an engineering subsystem, was used to optically
      navigate the spacecraft upon approach to the comet. This process
      allowed the spacecraft to achieve the proper flyby distance, near
      enough to the nucleus, to assure adequate dust collection for the
      prime mission and the best resolution for the extended mission. The
      camera also served as an imaging camera to collect science data. The
      data include high-resolution images of the comet nuclei at various
      phase angles during approach and departure. These images can be used
      to construct a 3-D map of the nucleus in order to better understand
      its origin, morphology, and mechanisms, to search for mineralogical
      inhomogeneities on the nucleus, and potentially to supply information
      on the nucleus rotation state. The camera provided images that give
      information on the gas and dust coma during approach and departure
      phases of the missions. These images provide information on gas and
      dust dynamics, and jet phenomena, if they exist.
 
      In order to meet these science and optical navigation objectives
      the NAVCAM design was developed  utilizing a Voyager Wide Angle
      Optical Assembly. Additionally, the NAVCAM had a newly-developed
      scan mirror mechanism to vary the camera viewing angle and a
      periscope to protect the scanning mirror while the spacecraft
      flew through the comet coma. The NAVCAM was a framing charge
      coupled device (CCD) imager with a focal length of ~200 mm. The
      NAVCAM had a focal plane shutter and filter changing mechanism of
      the Voyager/Galileo type; the filter changing mechanism may have
      failed in flight (see Operational Considerations and Navigation
      Camera State History below) and was not used after that point. The
      detector was a charge coupled device (CCD), cooled to suppress dark
      current and shielded from protons and electrons. The electronics
      contained the signal chain and CCD drivers (located in the sensor
      head), command and control logic, power supplies, mechanism drivers,
      a digital data compressor and two UARTs to interface with the
      spacecraft Command and Data Handling (C&DH) subsystem. NAVCAM command
      and telemetry functions were also handled by the electronics
      including storage of science commands, collection of science imaging
      data and telemetry, transmission of imaging data and telemetry to
      C&DH and receipt of commands from C&DH. The NAVCAM used a data rate
      of 300 kpixels per second for transferring data to the C&DH. There
      was also the option for data reduction with 12-bit to 8-bit
      square-root compression, and windowing.
 
 
    Major Functional Elements
    =========================
 
      The NAVCAM comprised the following major functional elements
      (Newburn, et al., 2003 [NEWBURNETAL2003]):
 
        -  Optics
        -  Filter Wheel and Shutter Mechanisms
        -  Detector
        -  Scan Mirror Mechanism
        -  Periscope
        -  Electronics and NAVCAM Control
 
 
      Optics
      ------
        The optics subassembly inherited its hardware design from, and was
        built and tested for, the Voyager Project. It was a Petzval-type
        refractor lens with a ~200 mm focal length, f/3.5 and a spectral
        range of 380 nm - 1000 nm. The optical components, with the
        exception of the filters, were manufactured from LF5G15 and
        BK7G14 materials, which are radiation resistant.  A new field
        flattener element, located in front of the CCD window, was
        designed for Stardust to reduce field curvature and to provide
        additional CCD radiation shielding. The optics were supported on
        three invar rods that athermalized the system to keep the camera
        in focus over the operating temperature range. The optical
        barrel assembly mounted to the filter wheel and shutter assembly
        utilizing an aluminum truss structure. The housing and truss
        were also inherited hardware from Voyager. There was a small
        incandescent lamp, spider-mounted in front of the first lens
        element, that could be used for in-flight calibrations. Because
        radiation resistant optical materials were used to harden the
        optics, the lens had poor broad-band modulation transfer function
        (MTF) performance (axial color). The theoretical MTF for the
        spectral range 380 nm to 1100 nm was 30% at 32 lp/mm.  The
        thickness of individual filters was optimized to improve the MTF
        over the filter's passbands.
 
        Optics characteristics were:
 
          Focal length            200 mm
          Relative aperture       f/3.5
          Spectral Range          380 - 1100 nm
          Resolution              60 microradian/pixel
          Field of view           3.5 x 3.5 deg
 
 
      Filter Wheel Subassembly
      ------------------------
        The NAVCAM filter wheel assembly was inherited Flight Spare
        hardware from the Voyager Project. The assembly contained an
        eight-position filter wheel and a driving mechanism. To actuate
        the mechanism a pulse was sent that energizes the linear
        solenoid, thereby rotating the rocker arm by means of the
        connector rod. The pawl, pivoted on the rocker arm, was driven
        toward the next wheel cog. At this point the pawl released
        latch A from the cog wheel, extended the drive spring and then
        engaged the next cog on the wheel. This put the mechanism in
        the cocked position. When the solenoid was de-energized, the
        rocker arm and pawl were returned to their original positions by
        the drive spring, which advanced the filter wheel one position.
        During this travel the A latch followed the pawl inward and was
        in position to stop the filter wheel at the end of the stroke.
        The back latch B ratcheted over the cogs, preventing the wheel
        from back lashing. A series of photo-diodes were uncovered by a
        pattern of small apertures in the filter wheel, which were unique
        for each filter position. Thus the filter that was in the
        optical path was known for each image taken and was included as
        part of the engineering telemetry.
 
        The spectral response of the camera was controlled by bandpass
        filters. The bandpass filters for Stardust were new and
        installed into the filter wheel to replace the Voyager filters.
        In this table, the filters are identified along with some of
        their characteristics and their position location in the filter
        wheel:
 
        (SDN:  as noted elsewhere only the OPNAV filter was ever used
        after a failure early in the prime mission.
 
        The /DATA/FILTRANS/ directory of the data set now also contains
        NAVCAM Filter Transmission tables, and the confusing Blocking
        entries have been removed from the table below.)
 
 
          Filter Name               OPNAV -- Optical Navigation
          Central or Passband (nm)  698.8
          FWHM(nm)                  400
          Transmission              92%
          Wheel Position            0
 
          Filter Name               NH2 -- NH2 Emission
          Central or Passband (nm)  665.1
          FWHM(nm)                  15
          Transmission              70%
          Wheel Position            1
 
          Filter Name               OXYGEN -- Oxygen (0[1D]) Emission
          Central or Passband (nm)  633.6
          FWHM(nm)                  12
          Transmission              60%
          Wheel Position            2
 
          Filter Name               C2 -- C2 (C2 delta v=0 band)
          Central or Passband (nm)  513.2
          FWHM(nm)                  12
          Transmission              65%
          Wheel Position            3
 
          Filter Name               YELLOW -- Yellow Continuum
          Central or Passband (nm)  580.2
          FWHM(nm)                  4
          Transmission              50%
          Wheel Position            4
 
          Filter Name               RED -- Red Continuum
          Central or Passband (nm)  712.9
          FWHM(nm)                  6
          Transmission              70%
          Wheel Position            5
 
          Filter Name               NIR -- NIR Continuum
          Central or Passband (nm)  874.6
          FWHM(nm)                  30
          Transmission              70%
          Wheel Position            6
 
          Filter Name               HIRES -- High Resolution
          Central or Passband (nm)  596.4
          FWHM(nm)                  200
          Transmission              85%
          Wheel Position            7
 
        All wavelengths are in nanometers.
 
      Shutter Subassembly
      -------------------
        The NAVCAM shutter assembly was also inherited Flight Spare
        hardware from the Voyager Project. The device was a two-blade
        focal plane mechanism. Each blade was actuated by its own
        permanent rotary solenoid. The duration of the exposure was
        controlled by the time interval between two pulses (an open
        pulse and a close pulse). The open pulse powered the 'leading'
        blade and the close pulse powered the 'trailing' blade. The
        exposure sequence started with the leading blade covering the
        aperture. An open pulse moved the leading blade, uncovering the
        aperture, and the close pulse moved the trailing blade, in the
        same direction, covering the aperture again. The permanent
        magnets in the rotary solenoid of each blade held the blades in
        a detent position when the shutter was not powered. Exposures
        could be taken with the blades moving in either direction. A
        total of 4096 exposure times were available that ranged from 5 ms
        to 20s, in 5ms increments. There was also a bulb command, for
        longer exposures, that allowed the shutter to be held open for
        any desired length of time.
 
        This double-bladed shutter had the property that in one direction
        the exposures are 1.4 ms shorter, and in the other direction are
        0.4ms longer, than commanded.  Therefore, a setting of 5ms, which
        was the shortest possible, resulted in alternate 5.4ms and 3.6ms
        exposures, those at 25 ms, alternate 25.4ms and 23.6ms exposures,
        and so on.  This asymmetry is referred to as the shutter polarity,
        with the two directions designated forward (FWD) and backward
        (BCK).  Occasionally bias frames, for which the commanded exposure
        is zero and so for which also the shutter does not move, are taken
        for transmission to Earth.  Bias frames do not change the shutter
        polarity.
 
        SDN: Another zero-exposure operation which does not change shutter
        polarity was a readout of the CCD without storing the resultant
        pixel data.  This was performed four times as part of each normal
        NAVCAM power-on sequence.  It was also used as a keep-alive
        command, executed every 361s while the NAVCAM was powered on, to
        prevent the triggering of an automatic timeout which put the
        instrument into a low-power mode.  In the low-power mode the NAVCAM
        could not be commanded or otherwise returned to an operational
        state except by powering it off and then on again.
 
        Extensive analysis of images from the Stardust prime mission,
        as well as calibration images taken during the Stardust-NExT
        extended mission, further refined the knowledge of the shutter
        performance.  In the end a polarity-dependent and image
        line-dependent model was developed to model the actual exposure
        time of each pixel in an image.  It was also discovered that
        zero-exposure frames, such as bias frames or keep-alive CCD
        readouts, do not change the polarity of the shutter (as had been
        stated in the prime mission version of this catalog).  See the
        calibration documentation for further details.
 
 
      Detector
      --------
        The NAVCAM used a charge coupled device (CCD) detector packaged
        for the Cassini Imaging Science Subsystem (ISS). The typical
        operating temperature range was -55 C to -15 C. The CCD was mounted
        in a hermetically sealed package, which was back-filled with argon.
        An operating temperature of around -35 C was needed for suppression
        of dark current and to minimize proton gamma and neutron radiation
        effects. The NAVCAM employed passive radiative cooling to maintain
        the detector operating temperature.
 
        NAVCAM detector characteristics were:
 
          Format               1024 x 1024 pixels
          Pixel size           12 x 12 micrometers
          Full well            >= 100,000 e-
          Dark current         < 30 e-/pixel/sec at operating temperature
          Charge transfer efficiency  0.99996 at operating temperature
          Read Noise           <= 90 e- rms
 
 
      Scan Mirror Mechanism
      ---------------------
        This mechanism enabled the stationary wide angle optics (flying
        sideways during encounter) to keep the comet in view during
        flyby. The scanning mirror, located some distance forward of
        the camera lens faced 45 degrees away from the camera viewing
        axis. Rotating the mirror about the camera axis at the proper
        rate enabled comet tracking during flyby. The mechanism was a
        single degree of freedom device. It required proper spacecraft
        orientation so that the comet could be viewed in a viewing plane
        originating at the scan mirror and oriented perpendicular to
        the camera axis. The initial forward looking view (0 degree
        position) was through a periscope which protected the scan
        mirror. The mirror's home position was at -20 degrees, at which
        the camera saw a black object on the spacecraft. Total mirror
        rotation was 220 degrees, allowing views up to 20 degrees beyond
        looking straight back. The maximum rotational rate was
        approximately 3.1 degrees/sec.
 
        The mechanism comprised a cylindrical section with mirror and
        an anti-backlash mechanism, the drive unit with motor, gearbox
        and slip clutch and a base that housed the control
        electronics. The cylindrical section was coaxial with the camera
        lens. It comprised the rotational housing containing the
        mirror and a stationary housing with an anti-backlash mechanism
        attached to it. The sections of the housing that held the main
        bearings were made from titanium to enable accurate operations
        over a 100-degrees C temperature range. A smooth rotational
        motion was further assured by a duplex bearing pair, by
        precision gears and an anti-backlash mechanism utilizing a
        negator spring to produce a constant torque against the
        rotational motion. This performance should have limited pixel smear
        to approximately 2 pixels. The mirror, made of zerodur, was bonded
        to flexures that attached to the rotational housing. Baffling
        rings along the optical path reflected some, but not all, stray
        light away from the lens.
 
        The drive unit next to the housing comprised the following
        components.  A brushless DC motor from American Electronics
        Inc.:  Vmax=36V, T=10oz-in, n~1200rpm. This motor was previously
        space qualified for the MISR project. The motor was flanged onto
        the four stage planetary gearbox made by American Technology
        Consortium: e=252.6:1. The gearbox was previously space
        qualified for the Mars Pathfinder project. A slip clutch at the
        gearbox output shaft utilized a set of Belleville springs to
        keep the pinion's transmitted torque within a predetermined
        limit. It prevented mechanical damage in the event of control
        failures that might cause the mechanism to over-rotate and hit
        the stops that limit travel. The pinion was engaged with the
        main gear on the rotational part, providing a fifth
        transmission stage. The overall gear ratio was 2518.6:1.
 
 
      Periscope
      ---------
        The periscope was an optical assembly that allowed the scan
        mirror to look over the protective Whipple shield while it was
        pointed forward, in a direction parallel to the spacecraft +X
        axis. This was to protect the scan mirror from particle
        impingement, that would significantly degrade its performance,
        during cruise, upon approach and while flying through the comet
        coma. The periscope contained two rectangular mirrors mounted at
        45 degrees with respect to the space craft +X axis.
 
        The mirrors were made out of aluminum to reduce the rate and amount
        of degradation from particle impacting. For light weighting, the
        mirrors were fabricated using an aluminum foam core composite
        material with solid face sheets brazed onto the front and back
        surfaces. Single point diamond turning was used to figure the
        reflective surface of the mirrors. Since the forward looking mirror
        was exposed to the impacting particles, it was post polished and
        received only a very thin protected aluminum coating, while the
        mirror facing away from the particle stream was nickel coated and
        post polished with a thin protected aluminum coating. This process
        achieves a much better mirror figure and smoother surface finish,
        but the coating tends to flake off when exposed to particle impact.
 
        The periscope structure was a graphite/epoxy composite
        construction. This material was chosen to make the structure
        light and to reduce thermally induced distortions from the
        spacecraft to the periscope assembly. Each mirror was
        kinematically mounted to the composite structure using three
        triangular bipod flexures. The periscope was only utilized when
        the scan mirror was looking forward. After the scan mirror had
        rotated approximately 15-20 degrees down toward the spacecraft
        -Z axis, it was no longer imaging through the periscope. The
        periscope was designed so that the images taken while the
        mirror was partly looking through the periscope could still be
        used for optical navigation.
 
        SDN:  The calibration effort further refined the understanding
        of the periscope's effect on science imaging.  See the calibration
        documentation for further details.
 
 
      Electronics and NAVCAM Control
      ------------------------------
        The electronics for the NAVCAM comprised two major parts: the
        camera electronics and the scan mirror electronics. The sensor
        head electronics (part of the camera electronics) were mounted
        on a chassis that was located behind the focal plane of the
        optics, while the rest of the camera electronics and the scan
        mirror electronics were housed in the baseplate support. The
        NAVCAM electronics controlled NAVCAM functions and process NAVCAM
        commands and telemetry. The NAVCAM electronics were powered from
        the spacecraft 28-volt regulated and 34-volt unregulated power
        supplies.
 
        The portion of the camera electronics mounted behind the camera
        was called the sensor head electronics. These electronics
        supported the operation of the CCD detector and the preprocessing
        of the detector data. The pixel data were quantized to 12 bits
        giving an intra-frame dynamic range of 4096. Detector readout
        rate was fixed at 300 kpixels / second. In addition, a direct
        access port was included in the sensor head electronics to send
        telemetry to the NAVCAM ground support equipment. This port was
        used for ground testing only.
 
        The remainder of the camera electronics was called the main
        electronics. The main electronics provided the power and performed
        all NAVCAM control functions. These electronics included a CCD
        clock generator, image compressor, image buffer, mechanism and lamp
        drivers, telemetry mux and converter, bus controller, UARTs and
        power supplies. The spacecraft-specified RS-422 Bus was used for
        communication with the Command and Data Handling (C&DH) unit. A
        high-speed bus was used for transmission of image data, and a
        low-speed bus was used for sending and receiving commands and
        telemetry.
 
        The NAVCAM scan mirror mechanism had its own interface with the
        spacecraft.  This included a separate power interface, a
        bi-directional low-speed RS-422 bus for telemetry and
        commanding transmission, a low-speed RS-422 bus for outputting
        motor rotation pulses, and a discrete output for motor
        direction. All interfaces with the scan mirror mechanism were
        done through one 24 pin connector designated J2 that was mounted
        in the NAVCAM baseplate.
 
 
    NAVCAM Commanding and Operational Modes
    =======================================
 
      All commands were transmitted and received by the NAVCAM over the
      low-rate RS-422 bus. Commands received by NAVCAM were echoed back
      to the spacecraft, including parity errors, so that commands with
      errors could be ignored. This table contains a list of NAVCAM
      commands:
 
        Discrete Commands:
 
          Command                       States/Contents
          ---------------------------   ---------------------------------
          Camera power off              Turn camera power off
          Camera power on/reset state   Turn camera power on/reset camera
 
          Camera Function Commands:
 
          Sample Analog telemetry       1 of 8 possible channels
          Sample Digital telemetry      8 registers
          Move filter wheel             1- 8 positions
          SDN: Readout CCD              -
          Take picture (exposure time)  shutter exposure and return image
                                        data/digital telemetry
          Select analog telem channel   1 of 8 possible channels
          Calibration lamp              On or Off
          Data compression              On or Off
          Shutter bulb mode             Open or close
 
        Scan Mirror Commands:
 
          Command                       States/Contents
          ---------------------------   ---------------------------------
          Sample telemetry              4 registers
          Move mirror                   Mirror was rotated at specified
                                        velocity
          Scan Motor power              On or Off
          Scan Mirror Heater            On or Off
 
      SDN:  N.B. Mission Operations provided a detailed log of camera
      commanding, which was essential in determining shutter polarity and
      other camera state parameters used in NAVCAM data calibration.  See
      the calibration documentation for further detail.
 
 
    Telemetry Collection
    ====================
 
      The NAVCAM collected pixel data, engineering data and status
      data. These data were divided into three categories:
 
        Camera Digital:
          Image data
          Shutter exposure time
          Lamp status (on/off)
          Compression status (on/off)
          FIFO status
          Filter Wheel move steps
          Filter Wheel position
 
        Camera Analog:
          Filter Wheel voltage
          CCD Temperature
          + 5 Volt supply voltage
          - 5 Volt supply voltage
          + 12 Volt supply voltage
          - 12 Volt supply voltage
 
        Scan Mirror
          Mirror velocity
          Scan motor status (on/off)
          Heater Status (on/off)
          Motor direction
          Motor rotation pulses (tick marks)
 
      Housekeeping telemetry comprised engineering and status data
      only, packetized with appropriate header information into packets
      called housekeeping packets. This telemetry was used when the
      NAVCAM was in an ON power state. This telemetry was only used when
      the NAVCAM was actively taking data.
 
 
    Effective Data Rates
    ====================
 
      NAVCAM electronics provided a single data rate of 300 kilo-pixels
      per second.
 
 
    Encoding and Compression
    ========================
 
      The pixel data from the NAVCAM could be processed within the NAVCAM
      in several ways. The default processing was to transmit the
      converted 12-bit data. When data compression was turned on, the
      12-bit data were compressed to 8 bits using a square-root compression
      algorithm. This was accomplished via a look-up table stored in
      ROM.
 
      SDN:  N.B. The compression look-up table archived in early versions
                 of the Stardust prime mission PDS archived NAVCAM data
                 sets had an error in it; this was discovered during the
                 calibration activities for Stardust-NExT.
 
 
    Power Management
    ================
 
      The camera electronics were required to draw less than 8 watts, and
      the scan mirror less than 10 watts, steady state. Operational
      constraints were placed on the NAVCAM to limit the power drawn by
      NAVCAM from the spacecraft. This table contains a list of the power
      operating states.
 
        State           Definition
        ------------    ------------------------------------------------
 
        Camera Off      28-volt power to the NAVCAM was off. Heaters
                        powered directly by the spacecraft could still
                        be on.
 
        Camera On       28-volt power was applied to the NAVCAM to
                        receive commands, send telemetry and take data.
 
        Scan motor Off  Power supply to scan mirror was off. Heater could
                        still be on.
 
        Scan motor On   Power was applied to scan motor to receive
                        commands, send telemetry and scan.
 
 
      At power turn on, the NAVCAM registers were all set to zero. At
      this point the camera was in an 'idle mode' with all clocks
      running, waiting to receive commands. The camera remained in this
      state until the first command was received. The states of all
      mechanisms were what they were when the camera was last turned
      off, except that the shutter polarity was reset.
 
 
    NAVCAM Safe State
    =================
 
      In response to a concern that the NAVCAM boresight may, in a
      spacecraft fault condition, be exposed to the sun (accidentally
      incident sunlight), a method to protect the shutter and focal
      plane of the camera was developed. The NAVCAM safe state was
      defined as placing a narrow band filter in the optical path and
      opening the shutter. To reset the NAVCAM to a normal operating
      state, a power-on reset cleared the FPGA lockup.
 
 
    Operational Considerations and Navigation Camera State History
    ==============================================================
 
      Two years after launch the NAVCAM suffered its one known failure
      when the filter wheel refused to move when commanded.
      Fortunately for the overall success of the STARDUST mission, it
      stuck on one of the two wide-bandpass filters, the OpNav
      (Optical Navigation) filter, a filter that transmitted light from
      about 400 to 900 nm and had the greatest total throughput of any
      of the eight filters. This filter served most engineering needs
      perfectly well. The camera, however, had a Petzval lens system,
      and over such a wide wavelength range suffered from some
      chromatic aberration. As a result, the intrinsic point spread
      function was about 1.3 pixels FWHM (the high-resolution filter,
      by comparison, had a point spread function of a quarter pixel).
      Further, this camera lens was manufactured in the early 1970s
      for the Voyager program, and its antireflection coatings 30
      years later left something to be desired. As a result, all
      images exhibited a broad shallow skirt of scattered light.
 
      When first used after launch, the camera was observed to be
      heavily contaminated by a coating of unknown source and
      composition. Total sensitivity was down by a factor of almost
      100. A mild heating of the detector to 9 C for 143 hours,
      utilizing an internal heater, resulted in a slight improvement in
      performance, reducing the sensitivity loss to about a factor of
      ten. Every star image still showed a huge halo of scattered
      light.  Turning the spacecraft to place direct sunlight on the
      radiator, normally used to cool the detector, raised the detector
      temperature to 24 C for 30 minutes and resulted in great
      improvement. The camera then showed sensitivity approaching that
      originally expected and significantly reduced scattered light.
      Following passage through perihelion and Earth gravity assist,
      images were acquired of the Moon and of star fields for geometric
      calibration. It was obvious that some re-contamination had
      occurred during the previous three months when the spacecraft
      (but not the cooled detector) was warmest. A third heating cycle
      resulted in the best images since the camera left the calibration
      laboratory. A five-second exposure reached magnitude 11.7 with a
      signal to noise of three. The point spread was essentially the
      1.3 pixels expected for the filter, though there was still a
      broad, very shallow, skirt of scattered light caused by internal
      reflections in the lens and by residual contamination. Camera
      performance remained essentially constant for the next six
      months.
 
      After a year in deep space where power was low, communication
      bandpass limited, and no imaging was attempted, a calibration
      lamp image once again showed small re-contamination.
      Interestingly, the periscope, which was not used for most imaging,
      showed great improvement compared to two years earlier. Before
      beginning the Annefrank approach, 60 hours of heating to a
      temperature just above freezing was carried out with the internal
      heater. No immediate check of the results of this heating cycle was
      possible, but was later performed before and after the Wild 2
      encounter.  Therefore, the Annefrank encounter was conducted as an
      engineering test and not to gather scientific data. Great caution
      must therefore be used when attempting to interpret the Annefrank
      images, since they do contain considerable scattered light.
 
      Images acquired May 21, 2003 showed that the camera resolution
      was still quite good, although a faint halo of scattered light
      appeared around each image. A calibration lamp image, taken on
      this date, showed loss in filament resolution, apparently caused
      principally by the scattered light. An image through the
      periscope was considerably improved over earlier images, but
      showed a great deal of scattered light on one side, presumably
      from the launch adapter ring that actually occulted a bit of the
      periscope on one side. A new feature was a line that was some 10
      DN above the background in column 221. This line appeared sometime
      between January 28 and May 21 and has remained until the final
      imaging in 2011.
 
      The project was not able to take new images until October 8 and
      18, 2003. These indicated that NAVCAM had acquired some 2.5
      magnitudes (a factor of ten) of obscuration over the previous 4.5
      months. Another heating cycle reduced this to about 0.5 magnitude.
      This state would have been adequate for the encounter but not
      what was desirable.
 
      On October 30, 2003 a new problem appeared. An image of the
      calibration lamp showed nothing. We did not know whether the bulb
      had burned out (something that had never happened before on any
      spacecraft) or the shutter didn't open (again something that
      had never happened before) or, after some thought, the
      possibility the solar flare that hit us at this time flipped a
      bit somewhere in the logic circuitry. The next images, taken on
      November 8, 2003 showed that the shutter was working just fine.
      There was concern that the failure of the lamp could indicate a
      short circuit somewhere, so the lamp was not tried again until
      after the Wild 2 encounter. At that time, January 13, 2004, the
      lamp was working just fine, leaving us with the somewhat unlikely
      conclusion that a solar particle had flipped a bit!
 
      Three images, each with a three-second exposure, taken on November
      13, 2003 were a first attempt to locate comet 81P/Wild 2. It hinted
      at being present in single images, but adding the three together
      convinced us that we had found 81P/Wild 2 on the first try.
      Images four days later with five-second exposures absolutely
      confirmed this. This began the optical navigation effort. Over
      the next month the images showed some degradation, and there was
      concern that this might hinder the final days of navigation, to
      say nothing of the quality of the comet images. So, just five
      days before the encounter, the Sun was once again turned on the
      CCD radiator for about 35 minutes. This procedure cleared things
      up beautifully.
 
      As the encounter approached, concern was expressed over the large
      number of on-off cycles the camera was undergoing for the optical
      navigation. It was decided to just leave the camera turned on, as
      a safety measure. Unfortunately this raised the CCD temperature
      by twelve degrees centigrade, and the images became loaded with
      hot pixels. (The optics and detector sit on top of the
      electronics box.) The hot pixels ruined the calibration run that
      was attempted on December 18, 2003. So, the camera was again
      turned on and off for every imaging sequence, which caused no
      problem. The camera went into its encounter activities in a very
      clean state and completed its imaging with great results. Another
      calibration sequence was attempted on January 13, 2004 with no
      problems, except that they were exposed on anything but a rich
      field. Post-encounter images through the periscope seemed to show
      it to have been heavily damaged by the particle bombardment during
      encounter, as was expected.  However, later testing showed no
      periscope degradation, and the 2004 results are attributed to
      scattered light.  And as mentioned previously, the calibration lamp
      was working just fine. Unfortunately this cal lamp frame was given
      a one second exposure rather than the appropriate 20 ms; every pixel
      was saturated.
 
      SDN:  Further calibration imaging and analyses have quantified some
      of the effects noted above.  See the following and the calibration
      documentation.
 
      NAVCAM fulfilled its duties admirably during the primary mission
      (Duxbury, et al., 2004; Tsou, et al., 2004; Brownlee, et al., 2004
      [DUXBURYETAL2004B] [TSOUETAL2004] [BROWNLEEETAL2004].
 
      The performance of the NAVCAM was monitored throughout the
      Stardust-NExT extended mission using a standard calibration sequence
      along with a few special calibrations.  Calibrations involved imaging
      of a variety of stars, several of which are photometric standards,
      acquiring dark frames, and taking images illuminated by the NAVCAM
      internal calibration lamp.  The problem with recurring camera
      contamination (Hillier, et al., 2011; Newburn, et al., 2003a & b;
      Tsou, et al., 2004; Li, et al., 2009 [HILLIERETAL2011]
      [NEWBURNETAL2003] [NEWBURNETAL2003B] [TSOUETAL2004] [LIETAL2009])
      was successfully controlled by periodic heating of the instrument
      using its internal electrical heaters and by placing direct Sunlight
      on the camera radiator.
 
      The cruise calibrations allowed characterization of camera imaging
      performance in the areas of geometric fidelity, spatial resolution,
      and radiometry (including zero-exposure signals, shutter times,
      linearity, field flatness, noise, and radiometric response rate) more
      accurately than had been possible during the primary mission.
      Preliminary radiometric calibration results have been incorporated
      into the image processing pipeline. Special observations allowed
      determination of the NAVCAM periscope throughput as a function of
      scan mirror angle, scattered light levels from the spacecraft
      structure as functions of mirror angle and the Sun illumination
      direction on the spacecraft, and charge bleeding and residual image
      in the CCD detector.
 
      Calibration sequences similar to the standard cruise calibration were
      executed eighteen days and ten days before Encounter closest approach
      (E-18d and E+10d).  The NAVCAM performance remained essentially
      unchanged throughout the Stardust-NExT mission.  A publication with
      more complete NAVCAM calibration results is available (Klaasen,
      et al., 2011 [KLAASENETAL2011B]).
 
      NAVCAM imaging of Tempel 1 was initiated at E-60d and was repeated
      twice per week.  Exposures of 10s and 20s (the maximum commandable
      by the spacecraft) were used; however, the comet was not bright
      enough to be detected in the initial images even after summing all 8
      images taken at each sampling time.  Many frames had several pixels
      of smear using these long exposure times.  At this time, the
      spacecraft was oriented with its dust shields pointed away from the
      comet (to avoid having to image it through the periscope) and with
      the high-gain communication antenna pointed at Earth to allow data
      downlinking.  As the spacecraft range to the comet decreased, the
      mirror angle required to view the comet progressively increased.
      When it exceeded 168deg, increasing levels of scattered light began
      to raise the background signal and decrease the signal-to-noise ratio
      (SNR).  Starting on E-27d, the mirror was moved back to 160deg, and
      the spacecraft was maneuvered off Earth point to view the comet.
      This reduced the scattered light and allowed the first detection of
      the comet in stacks of 8 summed images.  Daily 8-frame image sets of
      351x351-pixel subframes were typically acquired after this time.
      These images were usable for optical navigation, but the SNR was
      still too low for useful science.  At E-7d, the spacecraft was
      flipped around to put the dust shields forward, and the scan mirror
      was set at 20deg for comet imaging.  The comet SNR in 8-frame stacks
      became scientifically useful at about this time, and sets were taken
      every 2 hours from this point until E-2d when approach imaging was
      halted to prepare the spacecraft for the encounter.  Evidence of the
      nucleus brightening the central pixel was first seen at about E-3d.
 
      The close encounter image set was restricted by spacecraft memory and
      software to 72 full-frame compressed images, as had also been the
      case at Wild 2.  These images were sequenced to occur within E+/-4m
      (minutes).  Images were taken on 8-s centers outside E+/-144s
      (seconds) and on 6s centers inside that period.  Scan mirror pointing
      was controlled by the onboard autonomous navigation software, which
      worked flawlessly to keep the nucleus in the camera FOV.  The pixel
      scale in the encounter image set ranged from 158 m/pixel down to
      11m/pixel at closest approach.  Four of the 72 images (the first,
      last, and those at E+/-72s) were intentionally overexposed to allow
      better detection of any near-nucleus jets.  Other than those frames,
      nearly all images were well exposed.  Slight saturation of the bright
      limb occurred on two frames (E-33s and E-15s) due to the actual
      arrival time being 15s earlier than nominal.  The first 24 images
      viewed the comet through the periscope; 6 of those frames showed
      evidence of double images, as expected for mirror angles between 8
      and 15deg, where light reaches the camera both through the periscope
      and from just outside it.  No evidence of any optical contamination
      was observed.
 
      Departure imaging resumed at E+1d.  With the dust shields forward,
      the scan mirror angle began at about 174deg.  Significant scattered
      light was apparent, but the SNR was adequate for continued useful
      science.  Single 351x351-pixel subframes were acquired every 5
      minutes to support high-time-resolution monitoring of coma activity.
      Increased central pixel brightening due to the nucleus was no longer
      seen after about E+5d.  At E+7d, the sampling rate was decreased to
      every 11 minutes due to decreasing Deep Space Network ground
      receiving station coverage, and the subframe size was reduced to
      201x201 pixels one day later.  The scattered light level gradually
      decreased with time, as did the comet signal.  Useful science imaging
      was no longer achieved after E+10d, and comet imaging was then
      terminated.  All approach and departure images were acquired
      uncompressed.  No evidence of optical contamination was observed
      except for the residual contamination seen after the last heating
      procedure during cruise.
 
 
   References
   ==========
 
      Brownlee, D. E., et al., The Surface of young Jupiter family comet
      Wild 2:  View from the Stardust spacecraft, Science, v. 304, no.
      5678, pp. 1764-1769, June 18, 2004.
 
      Duxbury, T. C., et al., The Asteroid 5535 Annefrank size, shape, and
      orientation:  Stardust first results, JGR-Planets, v. 109, issue E2,
      article E02002, Feb. 6, 2004.
 
      Hillier, J. K., et al., Photometric modeling of Asteroid 5535
      Annefrank from Stardust observations, Icarus, v. 211, pp. 546-552,
      2011.
 
      Li, J-Y, et al., Photometric analysis of the nucleus of Comet
      81P/Wild 2 from Stardust images, Icarus, v. 204, pp. 209-226, 2009.
 
      Klaasen, K. P., et al., Stardust-NExT NAVCAM calibration and
      performance, submitted to Icarus, 2011
 
      Newburn, R. L., et al., Stardust Imaging Camera, JGR, v. 108, no.
      E10, pg. 8116, 2003a.
 
      Newburn, R. L., et al., Phase curve and albedo of asteroid 5535
      Annefrank, JGR, v. 108, no. E11, pg. 5117, 2003b.
 
      Tsou, P., et al., Stardust encounters comet 81P/Wild 2, JGR, v.
      109, E12S01, 2004.

        