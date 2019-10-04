# 0.2.0 (Unreleased)

* Renamed `bin/focus.ctfapply` to `bin/focus.ctf`
* Added option `--randomize_beyond` to `focus.postprocess`
* Added options `--transparent` and `--svg` to `focus.ctf`
* Included `bin/focus.resample`
* Included `bin/focus.project`

# 0.1.4

Fixed default argument bugs in `AutoMask()` of `focustools/util.py`

# 0.1.3

Fixed x-label in CTF plots of `bin/focus.ctfapply`

# 0.1.2

Another bugfix in `focustools/util.py`

# 0.1.1

Bug fixes in:

* `bin/focus.ctfapply`
* `bin/focus.mrcz`
* `focustools/util.py`
* `RELEASE_NOTES.md`

# 0.1.0

Initial release containing:

* `bin/`  
  * focus.ctfapply  
  * focus.mrcz  
  * focus.postprocess  

* `focustools/utils.py`  
  * AdhocSSNR(imsize=[100, 100], apix=1.0, DF=1000.0, WGH=0.1, Cs=2.7, kV=300.0, S=1.0, F=1.0, hp_frac=0.01, lp=True)  
  * AutoMask(img, apix=1.0, lp=-1, gaussian=False, cosine=True, cosine_edge_width=3.0, absolute_threshold=None, fraction_threshold=None, sigma_threshold=1.0, expand_width=3.0, expand_soft_width=3.0, floodfill_rad=-1, floodfill_xyz=[0, 0, 0], floodfill_fraction=-1, verbose=False)  
  * BackProject(img, pose=[0, 0, 0, 0, 0], interpolation='trilinear', pad=2, do_sinc=True, res_max=-1, apix=-1, return_weights=True, is_fft=False, DF1=1000.0, DF2=None, AST=0.0, WGH=0.10, invert_contrast=False, Cs=2.7, kV=300.0, phase_flip=False, ctf_multiply=False, wiener_filter=False, C=1.0)  
  * BandPassCrossCorrelation(img1, img2, apix=1.0, lp=-1, hp=-1, weights=None, rounding=True, eps=1e-8)  
  * CistemAutoMask(img, apix=1.0)  
  * CorrectCTF(img, DF1=1000.0, DF2=None, AST=0.0, WGH=0.10, invert_contrast=False, Cs=2.7, kV=300.0, apix=1.0, phase_flip=False, ctf_multiply=False, wiener_filter=False, C=1.0, return_ctf=False)  
  * CrossCorrelation(img1, img2)  
  * CTF(imsize=[100, 100], DF1=1000.0, DF2=None, AST=0.0, WGH=0.10, Cs=2.7, kV=300.0, apix=1.0, B=0.0, rfft=True)  
  * ElectronWavelength(kV=300.0)  
  * FCC(volume1, volume2, phiArray=[0.0], invertCone=False)  
  * FilterBfactor(img, apix=1.0, B=0.0, return_filter=False)  
  * FilterCosine(img, apix=1.0, lp=-1, hp=-1, width=6.0, return_filter=False)  
  * FilterDoseWeight(stack, apix=1.0, frame_dose=1.0, pre_dose=0.0, total_dose=-1, kv=300.0)  
  * FilterGauss(img, apix=1.0, lp=-1, hp=-1, return_filter=False)  
  * FilterTophat(img, apix=1.0, lp=-1, hp=-1, return_filter=False)  
  * FilterWhiten(img, return_filter=False, ps=False)  
  * FirstZeroCTF(DF=1000.0, WGH=0.10, Cs=2.7, kV=300.0)  
  * FloodFilling(img, inimask, thr=0.0)  
  * FRC(image1, image2, phiArray=[0.0])  
  * FSC(volume1, volume2, phiArray=[0.0])  
  * Fsc2Xml(filename, x, y)  
  * GetFreqArray(NSAM=256, apix=1.0)  
  * GetNumberOfFourierSamples(imsize)  
  * HalfBitCurve(imsize=[100, 100], nsym=1, D=2.0, L=3.0, count=False)  
  * HighResolutionNoiseSubstitution(img, apix=1.0, lp=-1, random_seed=123456789, parallel=False)  
  * MaskAutoExpand(map1, map2, apix=1.0, init_lp=15, fraction_threshold=0.01, init_hard_edge=0, init_soft_edge=3, randomize_below_fsc=0.8, fsc_thr=0.143, random_seed=123456789, interp=False, verbose=False)  
  * MatchAmplitudes(img1, img2)  
  * MatchPowerSpectra(img1, img2)  
  * NormalizeImg(img, mean=0.0, std=1.0, radius=-1)  
  * Project(img, pose=[0, 0, 0, 0, 0], interpolation='trilinear', pad=2, do_sinc=True, res_max=-1, apix=-1, is_fft=False, DF1=1000.0, DF2=None, AST=0.0, WGH=0.10, invert_contrast=False, Cs=2.7, kV=300.0, phase_flip=False, ctf_multiply=False)  
  * RadialFilter(img, filt, return_filter=False)  
  * RadialIndices(imsize=[100, 100], rounding=True, normalize=False, rfft=False, xyz=[0, 0, 0], nozero=True)  
  * RadialProfile(img, amps=False)  
  * Resample(img, newsize=None, apix=1.0, newapix=None)  
  * Resize(img, newsize=None, padval=None, xyz=[0, 0, 0])  
  * ResolutionAtThreshold(freq, fsc, thr, interp=True, nyquist_is_fine=False, )  
  * Rotate(img, rot=[0, 0, 0], interpolation='trilinear', pad=1)  
  * RotateFFT(img, rot=[0, 0, 0], interpolation='trilinear', pad=1)  
  * RotationalAverage(img, nomean=False)  
  * Shift(img, shift=[0, 0, 0])  
  * SigmaCurve(imsize=[100, 100], sigma=3.0, nsym=1, D=2.0, L=3.0, count=False)  
  * SoftMask(imsize=[100, 100], radius=0.5, width=6.0, rounding=False, xyz=[0, 0, 0], rfft=False)  
  * VoxelsPerShell(imsize=[100, 100], count=False)  
