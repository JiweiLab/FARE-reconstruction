The details of code description can be found in the 'Code_description.pdf', and the following steps are a general procedure to run the 'DataForTest'.

1. Copy the 'PSF473.tif' to '\otf' folder (overwrite if existing).
2. Open the 'makeotf.m' and adjust the parameters in line 106-114, 
 choose the corresponding parameters. The test data are imaged with 473 nm wavelength and NA=1.2 water objective.
3. Run 'makeotf.m' and 3 files would be generated: 'OTF_exp.tif', 'OTFbead473.mat' and 'OTFbead473.tif'. 
Check the 'OTF_exp.tif', and if the 2 orders OTF both look like 'OTF_exp_example.tif', the OTF is OK. If not, adjust the 3rd and 4th parameter of 'ileavekz', or check your PSF.
4. Open the 'SireconDriver.m' and adjust the parameters. The details can be found in the 'Code_description.pdf'.
Generally, you should 
1) Adjust the paths of 'ifiles', 'ofiles' and 'otffiles'. For time serials data, each time point should be one file, and 'ofiles' should be file name without last number.
2) Choose the right wavelength and 'na'.
5. Run 'SirenconDriver.m' and a folder named 'sr' would be generated, i.e. the reconstructed files. A folder named 'wf' may also be generated, i.e. the wide-field files.


