1 Advanced Optical Imaging Techniques for Biomedical Applications | 1.1 Advanced Optical Imaging for Blood Testing | Human Blood = Blood has four parts: red blood cells(oxygen carrier), white blood cells(immune respond), platelets(stop bleeding) and plasma(liquid component). = RBCs occupy 40-45% of the blood volume. lack a cell nucleus and most organelles.  Circulate for 100-120 days in the body. Red in color due to hemoglobin bind with oxygen = Hemoglobin (Hb) is an iron-containing oxygen-transport metalloprotein. EXAMPLE:{Pulse Oximeter for Monitoring Oxygen Saturation. Physical property 1 & 2: The amount of light absorbed is proportional to the concentration of the light absorbing substance; the length of the light path. Physical property 3: Oxy-Hb absorbs more infrared light than red light & Deoxy-Hb absorbs more red light than infrared light.} = Abnormal RBC count is often the first sign of an illness,as a part of complete blood cell (CBC) count. = FOMULA:{Total RBCs/µL = Number of RBCs counted * Dilution factor / (Area * Depth)} = A blood smear test involves examining a blood sample under a microscope after applying special stains. This test highlights the number, shape, and any abnormalities or changes in three types of cells: red blood cells, white blood cells, and platelets. = Current gold-standard method for malaria diagnosis is examining blood films using an optical microscope. = WBCs' Abnormalities in the number and shape are usually associated with infections. = {WBC Count Associated Diseases: Monocyte - High: Chronic infection. Low: Not typically suggest a medical condition. Granulocyte - High: Leukemia, Allergic reactions, Acute infection. Low: Bone marrow cancers, Autoimmune disorders, Aplastic anemia. T Lymphocyte and B Lymphocyte - High: Acute infection, Lymphocytic leukemia. Low: Autoimmune disorder, HIV, Tuberculosis, Hepatitis, Flu.} | 1.2 Optical Coherence Tomography {Tomogram: a two-dimensional image representing of a slice or section through a three dimensional object. i.e., cross-sectional image. Combining these tomograms we can get a three-dimensional structure of the object.} {OCT vs. Ultrasound: OCT uses light and low-coherence interferometry to determine the time delay of reflections, whereas ultrasound uses sound waves. OCT has 10-100 times better axial resolution than ultrasound or MRI due to shorter and faster light waves. OCT images have 10 times more pixels per unit compared to ultrasound images.} {OCT Wavelength: Uses 600 nm to 2000 nm, where tissue constituents exhibit low absorption. 2. Depth Resolution: High depth resolution is the main driving force behind OCT development. 3. Phase Relationship: Interference requires a strict phase relationship; multiple scattering events lose phase information. 4. Photodetection: Weak signals in the object arm are amplified by strong signals in the reference arm via photodetection. 5. Transverse Resolution: Determined by diffraction, as all OCT systems are built around a confocal microscope.} {OCT system comprises: 1.Viewing unit 2.Interferometric unit 3.Computer display 4.Control panel 5.Color inkjet printer} | 1.2 Optical Diffraction Tomography. 

2 Magnetic Resonance Imaging | 2.1 Overview {Physics of MRI: MRI is based on nuclear magnetic resonance (NMR), describing the magnetic behavior of atomic nuclei with an odd number of protons. The human brain's high water content makes hydrogen (1H), with a single positively charged proton, the most abundant nucleus used in MRI. Other nuclei such as 13C, 31P, 23Na, and 19F are also detectable with MRI.} {When an external magnetic field 𝐵 is present or applied, the spins in a spin system exhibit a weak tendency to precess} {Precession in MRI refers to the spinning motion of nuclei in a magnetic field at the Larmor frequency (proportional to the field strength, e.g., 128 MHz for 3T), producing a rotating magnetic field in the transverse plane within the RF range.} {T1 relaxation (spin-lattice relaxation) describes the exponential recovery of longitudinal magnetization to 63% of its maximum (M₀) after excitation, with the recovery time governed by the T1 constant: M(t) = M₀ × (1 − e⁻ᵗ/ᵀ¹).} {T2 relaxation (spin-spin relaxation) describes the exponential decay of transverse magnetization to 37% of its initial value due to spin phase desynchronization, with the decay time governed by the T2 constant: Mₜ(t) = Mₜ₀ × e⁻ᵗ/ᵀ².} {Contrast in MRI: By adjusting the sequence of RF pulses, different image types are generated. Repetition Time (TR) is the time between successive pulse sequences on the same slice, while Time to Echo (TE) is the time between the RF pulse and the received echo signal.} {T2-weighted image uses TE; T1 uses TR} {In MRI, T1-weighted images use short TR and short TE, T2-weighted images use long TR and long TE, and proton density-weighted images use long TR and short TE.} {For T1-weighted MRI, CSF is dark, WM is light, GM is gray, fat is bright, and inflammation is dark; for T2-weighted MRI, CSF is bright, WM is dark gray, GM is light gray, fat is light, and inflammation is bright.} | 2.2 fMRI Introduction {The Basics of BOLD fMRI: BOLD fMRI, the most common fMRI method, uses hemoglobin as an endogenous contrast agent, relying on magnetization differences between oxy- and deoxyhemoglobin. BOLD signals reflect neural activity, measure blood flow changes via the hemodynamic response, and show increased oxygenated hemoglobin with higher neural activation and glucose/oxygen supply.} {fMRI preprocessing minimizes artifacts, validates statistical assumptions, and standardizes brain region locations across subjects to enhance validity and sensitivity in group-level analysis.} {fMRI preprocess: 1.Slice-timing correction 2.Head motion correction 3.co-registration 4.spatial normalization 5.spatial smoothing} 2.3 fMRI Data Analysis | {Block design in fMRI averages brain activation over sustained periods (20–30 seconds) and contrasts it with resting state or comparison tasks to isolate the psychological process of interest.} {Event-related design uses short, randomized discrete events to measure time-locked brain activation, allowing selective averaging and post-experiment categorization of trials.} | 2.3.1 GLM {Task fMRI uses GLM (general linear model) to identify brain regions activated by specific tasks, treating data as a linear combination of known model functions (predictors) plus noise, with unknown amplitudes estimated from the data.} {The General Linear Model (GLM) is used in fMRI to analyze the relationship between experimental conditions and brain activity. The model represents voxel intensity as Y = BX + ε, where Y is the observed signal, X is the design matrix reflecting experimental conditions and their timing, B represents regression coefficients quantifying the contribution of each condition, and ε accounts for noise. The design matrix X is generated by convolving task timings with the hemodynamic response function (HRF) to model physiological responses. The regression coefficients (β) indicate the strength of brain activation under specific conditions and are used to compare brain activity across groups or tasks. GLM helps identify task-related brain regions and quantify the impact of different conditions on neural activity.} | 2.3.2 Brain Connectivity {Resting-state fMRI: a scan in which subjects relax (not sleeping) and told not to think anything} {Functional Connectivity: 2 or more fMRI time series asso in brain region} {Functional connectivity describes statistical relationships between brain regions without direction using Pearson Correalation, while effective connectivity reveals directed causal interactions between regions using Granger Casualty.} {Pearson’s Correlation is a normalized measure of linear relationship between two signals, ranging from -1 to 1, scale-invariant, and limited to detecting only linear correlations. Granger Causality identifies directed causal relationships between time-series data by determining if one signal improves the prediction of another, assuming temporal precedence.}

3 Nuclear Imaging 3.1 Overview {A nuclear medicine study requires a pharmacologic agent targeting specific organs, a radionuclide emitting detectable high-energy photons, and a device to capture and image these photons.} {Nuclear medicine basic principle involves injecting a tracer molecule carrying an unstable isotope, which participates in metabolic processes and emits gamma rays, allowing its concentration to be measured for analyzing organ function.} {}