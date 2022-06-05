The SDLPtools software implements a SLDP method for selective linkage disequilibrium pruning combined with biological prior information to increase th accuracy of genomic prediction.
The program can be compiled with perl on a unix or windows operating system using the following commands:
./SLDPtools --snpfile test_snpfile.txt --prior-snp-list test_prior_SNPlist.txt --r2 0.5 --window-size 50 --step-size 10 --out test_SLDP_out.txt

Options:
Use the “--help” option to display a list of options with a short description.
argument	type	description
--snpfile	[filename]	input snpfile file where missing genotype were not allowd
--prior-snp-list	[filename]	input snp_list file where each line is an SNPid
--r2	[num]	LD r2 threshold used in LD pruning
--window-size	[num]	the window size used in LD pruning(SNP number)
--step-size	[num]	the step size used in LD pruning(SNP number)
--out	[filename]	filename for output

The folder of Test_data includes simulated data for testing purpose.
test_snpfile.txt: simulated genotype file.
test_prior_SNPlist.txt: simulated prior_SNPlist.
