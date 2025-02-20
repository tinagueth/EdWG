
 
    Instrument Host Overview
    =========================
 
    The LCROSS (Lunar CRater Observation and Sensing Satellite)
    mission was conceived as a low-cost means of determining the
    nature of hydrogen detected at the polar regions of the moon.
 
    LCROSS was selected as the Lunar Reconnaissance Orbiter (LRO)
    secondary payload on April 10th, 2006 and launched with LRO on
    June 18th, 2009.  To meet the requirements of a secondary
    payload, the LCROSS Shepherding Spacecraft (SSC) was built
    around an EELV Secondary Payload Adapter (ESPA) ring, originally
    designed as a mating interface for up to six small spacecraft or
    experiments as secondary payloads on Delta IV and Atlas V
    launches.  Developed by Northrop Grumman, the SSC featured five
    equipment panels and a solar array mounted radially at the ESPA
    mate ports.  A single monopropellant tank was mounted within the
    ESPA ring.  For launch, the nearly 900 kg (wet mass) LCROSS
    SSC was mated between the Centaur upper stage and LRO.
 
    The SSC utilized copies of several LRO avionics units, including
    its RAD750-based single-board computer, power and thruster
    control electronics, S-band communications electronics, and
    SpaceWire bus electronics.  LCROSS flight software derived
    heavily from software on previous programs, including EO-1 and
    WMAP.  LCROSS communicated in S-band via two omnidirectional
    antennas and two medium-gain antennas.  Transponder electronics
    enabled downlink at data rates up to 1 Mbps and uplink at 16
    kbps.  Following launch and LRO separation, attitude control was
    passed from the Centaur to the SSC.  The attitude control system
    (ACS) provided three-axis control using an inertial reference
    unit (IRU; no accelerometers), a star tracker, coarse sun
    sensors for emergency automated sun-relative attitude capture
    and tracking, and a set of eight monopropellant 5 N thrusters.
    Two additional 22 N thrusters provided orbit maneuvering
    capability.  The ACS featured twelve control mode/submode
    combinations, six tailored for specific operations while
    attached to the Centaur, and a second set for use after Centaur
    separation.  The LCROSS propellant tank contained just over 305
    kg of hydrazine for both attitude control and orbit maneuvering.
    The LCROSS power system featured a 368 W solar array and four 20
    A-h batteries.  LCROSS performed thermal control using a
    combination of resistive heaters, passive radiators, and
    multi-layer insulation.
 
    The LCROSS Payload
 
    The LCROSS Payload consists of nine science instruments, their
    supporting electrical, mechanical and optical harnesses, a
    central data handling unit (DHU) assembly, and thermal hardware
    (heaters, thermistors, and thermostats), all assembled onto the
    LCROSS spacecraft R6 Radiator Panel.  Eight of the nine science
    instruments are configured with their apertures in the +X
    direction (spacecraft body frame/SBF) and are accommodated in
    the Payload Observation Deck (POD).  The ninth instrument, near
    infrared spectrometer #2 (NSP2), has its entrance optical
    element orientated in the -Z direction (spacecraft body
    frame/SBF).  The Payload is located on the inboard side of the
    LCROSS spacecraft R6 Panel.
 
    Visible Camera
 
    The LCROSS visible camera (VIS) is a ruggedized analog video
    camera from the RocketCamTM camera family developed by Ecliptic
    Enterprises, Inc.  The unit consists of a camera module and a
    lens.  The camera's focal plane CCD sensor is 752 [H] x 582 [V]
    pixel format, operating at 30 Hz (60 fields/sec).  The flight
    unit's lens is a 12 mm (focal length), f/1.2 lens providing a
    30.1 degree [H] x 22.8 degree [V] (37.8 degree [Diagonal]) field-of-view.
    Interlaced NTSC fields are sampled by the Data Handling Unit
    (DHU) at 720 x 243 resolution resulting in a final image
    resolution of 720 x 486 pixels.  Each pixel is 24-bit RGB with 8
    bits per color channel.  These images are compressed using a
    lossy compression algorithm performed by the Analog Devices 611
    Video Codec set on 80% quality and decompressed on the ground.
    The LCROSS visible camera contains no cryogenic liquids or
    moving parts.  The visible camera's peak power during operation
    is 2.9 W.  The visible camera has been fixed to an
    auto-gain/white balance setting.
 
    Near-Infrared Cameras
 
    The LCROSS payload contains two near infrared (IR) (0.9-1.7 um)
    cameras (NIR1/NIR2).  Each camera consists of a Goodrich Sensors
    Unlimited model SU320-KTX and a CCTV lens. Each camera's focal
    plane InGaAs sensor has a 320 [H] x 240 [V] pixel format.  The
    25 mm, f/1.4 C-mount glass lens provides a 28.7 degree [H] x 21.7
    degree [V] (36.0 degree [Diagonal]) field-of-view.  Although the
    camera's native format provides 320 [H] x 240 [V] 12-bit images,
    the images are converted within the camera to an analog NTSC
    signal before transfer to the DHU where they are captured at 720
    [H] x 486 [V].  Due to similar processing within the DHU as
    needed for the VIS images, the two NIR camera images are
    captured as 24-bit per pixel RGB.  Because the NIR cameras
    provide grayscale images, the three RGB channels are identical
    except for noise introduced in the conversion to and from
    NTSC. These images are compressed in the DHU using a lossy
    compression algorithm performed by the Analog Devices 611 Video
    Codec set on 80% quality and decompressed on the ground.  In
    addition to a camera body and a lens, near infrared camera #1
    (NIR1) also contains a long-pass filter (wavelength > 1.4 um).
    NIR2, in comparison, is filter-less.
 
    Lenses for both cameras were provided by UkaOptics
    (http://www.ukaoptics.com/ #2514M) as part of the standard
    Goodrich package. These lenses are not optimized for the IR.
    The IR throughput of the lenses has not been documented, but is
    expected to be ~40%.  The near-infrared cameras contain no
    cryogenic liquids or moving parts.  There is an internal
    thermo-electric cooler that actively cools the InGaAs sensor.
    The manufacturer default settings for this cooler are used.
    Each camera's peak power during operation is 1.6 W.  Both gain
    and exposure times are configurable by commands sent to the
    camera.
 
    Mid-Infrared Cameras
 
    The LCROSS payload contains two mid-infrared (MIR) (6.0-13.5 um)
    cameras (MIR1/MIR2).  Mid-infrared camera #1 (MIR1) is a
    ruggedized vanadium oxide (VOx) microbolometer MIRIC TB2-30,
    from Thermoteknix Ltd.  Mid-infrared camera #2 (MIR2) is model
    ThermoVision Micron from Flir Systems/Indigo Operations.  Each
    camera's uncooled microbolometer focal plane sensor has a 164
    [H] x 128 [V] pixel format and is digitized at 14-bit
    resolution.  Each camera has a 30 mm, f/1.6 lens providing a
    15.0 degree [H] x 11.0 degree [V] (18.6 degree [Diagonal]) field-of-view.
    MIR1 also contains a 6-10 Om bandpass filter.  MIR2 is
    filter-less.  MIR1 is backfilled with dry Argon gas to prevent
    degradation due to humidity for terrestrial applications and
    does not contain any component volatile in vacuum.  Internal to
    both MIR modules is an instrumented-motorized shutter to provide
    a reference for temperature measurements.  Each camera's peak
    power during operation is 1.3 W.  A camera gain, which
    determines the sensitivity to temperature scenes (high gain: -20
    degC < T < +150 degC, low gain: +150 degC < T < +500 degC), is
    configurable with a command sent to the camera.
 
    Total Luminance Photometer
 
    The Total Luminance Photometer (TLP) provides visible light
    (400-1000 nm) intensity data at a 1000 Hz sampling rate.  The
    TLP instrument consists of two elements: (1) the Sensor
    Electronics Module (SEM), which contains the optics and sensor
    assembly and signal filtering, and (2) the Digital Electronics
    Module (DEM), which converts the analog sensor signal to a
    digital output, as well as higher order functionality.  The DEM
    is a commercial package that was modified for LCROSS.  This
    instrument is designed and manufactured by NASA Ames Research
    Center.  The optics in the SEM delivers an unobstructed ~10
    degree diameter field-of-view.  The TLP's sensor element is an
    uncooled Advanced Photonix, Inc.  (API) avalanche photo diode
    (APD) packaged in a dryair sensor container that can operate in
    a vacuum.  The TLP SEM is connected by an electrical harness to
    the TLP DEM.  The SEM and DEM are located within the Payload
    Observation Deck (POD) and on the R6 Panel, respectively.  The
    DEM is interfaced with the DHU (also on the R6 Panel) via a
    second cable, from which it is controlled.  The SEM and DEM's
    peak power during operation are 2.5 W and 12.0 W, respectively.
 
    Visible Spectrometer
 
    The LCROSS visible spectrometer (VSP) is a modified-commercial
    model from Ocean Optics Ltd., with its core operation based on
    their COTS QE65000 model.  It has been adapted for space use and
    is of similar design to a recently delivered spectrometer to Los
    Alamos for a Mars Science Laboratory (MSL) payload for launch in
    2011.  The VSP spectrometer design consists of an FC optical
    fiber input (0.11 NA) feeding a 25 micron x 1 mm entrance slit,
    where light is diffracted by a 1-inch f/4 optical cross
    Czerny-Turner spectrometer (grating 600 lines/mm, blazed at 350
    nm) with an oversized camera mirror.  The ~263-650 nm spectrum
    from the slit is imaged onto a 1044 x 64 pixel Hamamatsu CCD
    detector.  The data is co-added within the spectrometer,
    delivering a 16- bit, 1 x 1044 pixel spectra to the DHU
    electronics for packaging.  The first 1024 pixels contain
    spectral data.  The remaining 20 pixels contain provide
    temporally coincident but off-slit dark reference pixels.  The
    VSP resolving power is R~300, 500, and 850 at 300, 400 and 600
    nm, respectively.  The VSP contains no moving parts.  The CCD
    detector is cooled by an internal Thermoelectric Cooler (TEC),
    whose set point is programmable.  The VSP power is 4.8 W (TEC
    off), and can reach 11.8 W (at TEC setting -10 degC at operating
    temperature +19-20 degC).  Integration time (between 8 ms and 65.5
    s) is configurable.  Additionally, the VSP supports two
    operation modes - single and bracket spectra.  The former is a
    single spectra acquisition of the appropriate requested
    integration time.  The latter is a three-spectra acquisition
    defined by a base integration time and a multiplier that is
    divided or multiplied by the base integration time to yield a
    shorter or longer exposure time, respectively.  The VSP is fed
    by a 75 cm length 600-micron core-diameter UV/Vis glass fiber
    attached to a fore-optics unit in the POD.  This fore-optics
    unit (see below) is a fixed two-mirror and one lens system
    designed to provide a one degree diameter field-of-view.
 
    Near-Infrared Spectrometers
 
    The LCROSS payload contains two near-infrared spectrometers
    (NSP1/NSP2), located on the R6 Panel.  Their electronics units
    are identical, but they have different fore-optics designs.
    Near infrared spectrometer #1, NSP1, also known as the nadir
    NSP, is located inside the POD and its aperture is positioned in
    the +X direction (spacecraft body frame/SBF).  Near infrared
    spectrometer #2, NSP2, also known as the solar-viewer or
    occultation NSP, has its wide-field aperture centered along the
    -Z direction (spacecraft body frame/SBF).  Both spectrometers
    provide 1.20-2.45 um spectral coverage and nominal resolution
    0.035 um/pixel, yielding resolving powers R ~ 37-65 (NSP1) and R
    ~ 36-77 (NSP2).  Both spectrometers are manufactured by
    Polychromix, a company whose primary spectrometer line is
    designed for material analysis and chemical sensing.  The
    spectrometers are designed to take a single SMA NA=0.22 fiber as
    input instead of a slit, whose diameter defines the instrument
    resolution.  Since each spectrometer contains a single
    TEC-cooled InGaAs sensor element, a 1D-spectrum is created using
    an innovative electronically-tunable MEMS device that spatially
    masks the dispersed spectrum within the instrument.  This series
    of masks undergoes a digital transform on the ground to recreate
    the spectral information.  The spectrometer contains no moving
    parts (excluding the MEMS chip) and the peak power for each NSP
    is 2.5 W.  NSP1 and NSP2 are each fed by a single 600-micron
    core-diameter low-OH glass fiber of length 75 cm and 1.45 m,
    respectively, attached to a fore-optic.  The NSP1 fore-optics
    unit (see below) is located within the POD and is a fixed
    two-mirror and one lens system designed to provide 1 degree
    diameter field-of-view.  The NSP2 fore-optic (see below) is a
    diffuser providing ~130 degree fieldof- view, and is located external
    to the POD housing.  Both spectrometers have three modes, Impact
    Flash (IF), Hadamard Spectrum (HS) and Diagnostic Mode (DM),
    which are configurable by sending a command to the units.
 
    Fore-Optics and Fibers
 
    The LCROSS payload contains two fore-optic units and three
    fibers.  The three single-core fibers connect the electrical
    units of the three LCROSS spectrometers to their respective
    fore-optics (i.e., light-gathering optics).  All fibers are
    manufactured by Fiberguide Industries.  The two fore-optics, a
    dual-scope fore-optic feeding the NSP1 and VSP spectrometers and
    a diffuser fore-optic feeding the NSP2 spectrometer, have been
    designed specifically for the LCROSS mission by Aurora
    Technologies.  The dualscope fore-optic provides 1 degree
    diameter field-of-view (per scope) and a separation between the
    two scopes of < 0.1 degrees.  The diffuser fore-optic provides
    an unattenuated ~130 degree field-of-view.  The fibers were chosen to
    optimize for the band-pass and be compatible with the throughput
    and entrance optic requirements by the spectrometers.  For the
    VSP, the fiber is a 75 cm SuperguideG UV/VIS Spectral Range with
    NA=0.12+/-0.02.  For the NSPs, the fibers are AnhydroguideG Low
    OH fibers with NA=0.22+/-0.02, with lengths 75 cm and 145 cm for
    NSP1 and NSP2, respectively.  All three fibers have 600 Om
    core-diameters and are encased in a 1/8 inch (ID) stainless
    steel monocoil for ruggedization.
 
    Data Handling Unit
 
    The LCROSS Data Handling Unit (DHU) is a ruggedized video camera
    controller and data handling system based on the ruggedized
    Digital Video Systems (DVS) developed by Ecliptic Enterprises,
    Inc.  It captures and transmits compressed digital spectrometer,
    video and photometric data telemetry (in CCSDS format) from all
    nine instruments from the LCROSS science payload.  The DHU is a
    single conduction-cooled chassis designed to operate as
    independently as possible from its host vehicle.  In the
    limiting case, DHU operation is completely self-contained except
    for activation/deactivation commands that originate from the
    ground.  The DHU can store up to 10 slots of Non- Volatile
    Memory (NVM), which can be used for sequencing power and
    operational commands to the science instruments.  The DHU
    contains no moving parts, operates from the 32 V power supply by
    the spacecraft power bus, and its peak power during operation is
    13.5 W.  The DHU also provides the time-stamping function of all
    the science instruments and itself and provides error logs for
    when science data frames are dropped or corrupted due to
    bandwidth or performance issues.

        